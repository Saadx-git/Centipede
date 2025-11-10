# Centipede Game

A modern C++ implementation of the classic Centipede arcade game using SFML.

## Game Overview

Centipede is a fast-paced arcade shooter where you control a spaceship to destroy a centipede while avoiding enemies and obstacles.

## Features

- Classic Centipede gameplay with modern enhancements
- Multiple enemies: Centipede, Spider, Scorpion
- Interactive environment: Mushrooms and poisoned mushrooms
- Progressive difficulty with increasing levels
- Score system with high score tracking
- Smooth controls and responsive gameplay

## Prerequisites

Before running the game, ensure you have SFML 2.5+ installed.

### Installation Guides

Ubuntu/Debian:
sudo apt update
sudo apt install libsfml-dev

Windows:
1. Download SFML from https://www.sfml-dev.org/
2. Extract to C:\SFML\
3. Add C:\SFML\bin to your system PATH

macOS:
brew install sfml

## Installation & Running

### Quick Start
./make

This will compile and run the game automatically.

### Manual Compilation
If the make script doesn't work, compile manually:

g++ -c main.cpp -o main.o
g++ main.o -o centipede -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
./centipede

## Project Structure

centipede-game/
│
├── main.cpp
├── make
├── README.md
├── How to Play.txt
│
├── Textures/
│   ├── spaceship.png
│   ├── c_body.png
│   ├── c_head.png
│   ├── mushroom.png
│   ├── spider_score.png
│   ├── scorpion.png
│   ├── fire.png
│   └── pxfuel.jpg
│
├── Music/
│   └── field_of_hopes.ogg
│
└── minecraft/
    └── Minecraft.ttf

## Controls

W / Up Arrow    - Move Up
A / Left Arrow  - Move Left
S / Down Arrow  - Move Down
D / Right Arrow - Move Right
Spacebar - Shoot

## Game Elements

Player
- Spaceship that moves in the lower screen area
- Single bullet weapon system

Enemies
- Centipede: Main enemy that splits when segments are destroyed
- Spider: Fast-moving enemy with variable point values
- Scorpion: High-value target that poisons mushrooms

Environment
- Mushrooms: Destructible obstacles (2 hits to destroy)
- Poisoned Mushrooms: Lethal mushrooms created by scorpions

## Scoring System

Centipede Body - 10 points
Centipede Head - 20 points
Mushroom - 1 point
Spider (Close) - 900 points
Spider (Medium) - 600 points
Spider (Far) - 300 points
Scorpion - 1000 points

## Troubleshooting

Common Issues:

1. SFML not found:
export LD_LIBRARY_PATH=/path/to/SFML/lib:$LD_LIBRARY_PATH

2. Missing textures/music:
- Ensure all asset files are in the correct directories
- Check file paths in the source code

3. Runtime errors:
- Ensure all DLLs (Windows) or shared libraries are accessible
- Check asset file permissions

Developer: Saad Azhar
Email : daimazhar@gmail.com
Semester 1 - Project     FAST NUCES 

Enjoy the game!
