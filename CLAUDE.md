# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Chain Game is a single-file HTML5 canvas game. The entire game (v0.47) is contained in `index.html` with inline JavaScript - no build system, no dependencies, no npm.

## Running the Game

Open `index.html` in a browser. That's it.

For development, use a local server to avoid CORS issues with audio:
```bash
python3 -m http.server 8000
# or
npx serve .
```

## Architecture

### Single File Structure
Everything lives in `index.html`:
- HTML/CSS at the top
- All game logic in a single `<script>` block
- No modules, no imports, no bundling

### Core Game Objects
- `game` - Global game state (camera, pause, keys, coins collected)
- `player` - Position, velocity, carrying items/coins
- `post` - The central anchor point at (0,0)
- `chain` - Links connecting player to post (starts with 5 links)
- `npcs[]` - Array of all NPC definitions with dialogue, positions, items
- `modifiers` - Skill/ability modifiers (moveSpeed, carryCapacity, zoomOut, etc.)
- `skills` - Skill tree definitions (up/down/left/right)
- `jobs` - Courier and sorter job state

### Key Systems
1. **Chain Physics** - Inverse kinematics constraining player to post
2. **NPC Dialogue** - Multi-page dialogue with yes/no choices (Up/Down keys)
3. **Item System** - Abilities, diamonds, music disks, work tools, packages
4. **Music System** - Distance-based volume from music points (dB falloff)
5. **Save System** - localStorage auto-save on deposit

### Controls
- Arrow keys: Movement
- Left+Right simultaneous: Drop last item
- Up+Down hold (500ms): Switch music disk
- F: Fullscreen
- R hold (3s): Reset save

## Documentation Files

- `PARAMETERS.md` - All game constants and values
- `SKILLS.md` - Skill trees and NPC abilities
- `NPCS.md` - Complete NPC guide with locations and items
- `HISTORY.txt` - Version history and design decisions

## Development Notes

### Adding NPCs
NPCs are defined in the `npcs[]` array. Each NPC needs:
- `name`, `x`, `y`, `radius`, `color`, `outlineColor`
- `dialogue[]` - Array of pages, each page is array of 3 lines
- `itemType` - 'ability', 'diamond', 'musicDisk', 'straum', null
- `requiresCoins` - Cost (0 for free)
- `hasChoice` - true if yes/no dialogue needed

### Adding Music Disks
1. Add tracks to `music/[DiskName]/`
2. Create NPC with `itemType: 'musicDisk'`
3. Set `diskName` and `trackPaths[]`

### Debug Keys
- Key 9: Toggle work tools ability

### Style Guidelines
- Black and white aesthetic only
- Player/NPCs: Black circles with white outlines
- Items: Black circles with white outlines
- Packages: Black squares with white outlines
- Minimal, stylish, no color
