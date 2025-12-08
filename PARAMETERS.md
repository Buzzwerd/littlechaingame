# Game Parameters - Chain Game v0.48

## Canvas
- **Size**: 1000x800
- **Background Color**: #000 (black)

## Player
- **Radius**: 12
- **Fill Color**: #000 (black)
- **Outline Color**: #fff (white)
- **Outline Width**: 2
- **Base Speed**: 2
- **Base Slow Speed (carrying)**: 1
- **Base Acceleration**: 0.3
- **Base Deceleration**: 0.85
- **Starting Position**: (0, 20)
- **Starting Velocity**: (0, 0)
- **Slowdown Per Item**: 15% per item carried

## Post
- **Base Radius**: 15
- **Color**: #fff (white)
- **Position**: (0, 0) - world center
- **Pulse Alpha Range**: 0.3 - 1.0 (when carrying coin)
- **Pulse Base Speed**: 0.05
- **Pulse Max Speed**: 0.35 (at close proximity)

## Chain
- **Initial Links**: 5
- **Link Length**: 20
- **Segment Radius**: 8 (for collision)
- **Physics Iterations**: 5 (for rigidity)

## Coins
- **Radius**: 8
- **Color**: #fff (white)
- **Initial Spawn Count**: 200
- **Random Spawn Range**: 100 - 2500 (distance from post)
- **Reachable Coin Min Distance**: maxReach * 0.7
- **Reachable Coin Max Distance**: maxReach * 0.95

## Camera
- **Base Zoom**: 2.5
- **Zoom Interpolation Speed**: 0.05
- **CCC Offset Strength**: 0.5
- **CCC Offset Distance**: 100
- **CCC Offset Interpolation Speed**: 0.08
- **CCC Center Return Speed**: 0.95 (multiply by)

## Collision
- **Coin Pickup Distance**: player.radius + coin.radius (affected by pickup range modifier)

## Controls
- **Movement**: Arrow Keys (Up, Down, Left, Right)
- **Fullscreen Toggle**: F key
- **Drop Item**: Left + Right arrows simultaneously
- **Switch Music Disk**: Hold Up + Down for 500ms
- **Reset Save**: Hold R for 3 seconds

## Floating Text Effects
- **Font**: bold 24px monospace
- **Initial Velocity Y**: -1.5
- **Velocity Dampening**: 0.95 (multiply by)
- **Life Duration**: 1.0 (decreases by 0.015 per frame)

## Ability Display System
- **Display Delay**: 5.0 seconds before auto-dismiss
- **Countdown Skip**: Each arrow key press reduces countdown by 1 second
- **Overlay**: 85% black semi-transparent

## Visual Elements
- **Grid Dot Spacing**: 100
- **Grid Dot Radius**: 2
- **Footprint Interval**: Every 15 frames
- **Grass Bent Hold Time**: 180 frames (3 seconds)

## Music System
- **Music Min dB**: -42
- **Music Max dB**: 0
- **Default Music Range**: 1000 (3000 for post music)
- **Disk Switch Hold Duration**: 500ms

## Skill Modifiers
- **Movement Speed**: Additive percentage bonus
- **Movement Acceleration**: Additive percentage bonus
- **Movement Deceleration**: Additive/subtractive modifier
- **Carry Speed Penalty Reduction**: 0-1.0 scale (1.0 = no penalty)
- **Carry Speed Bonus**: Additive percentage bonus when carrying
- **Carry Capacity**: Additive coin count (base: 1)
- **Pickup Range**: Multiplier for coin pickup radius
- **Zoom Out**: Percentage reduction in zoom level
- **Camera Offset Reduction**: 0-1.0 scale (1.0 = no offset)

## Max Fulfillment System
- **Activation Threshold**: 10+ weight carried (coins + item weights)
- **Effect**: Speed boost when condition met

## Jobs System
- **Courier**: 3 deliveries per day maximum
- **Sorter/Retrieval**: Reset at 18:00 daily

## Brot's Animal Zone
- **Zone Radius**: 800px
- **Animal Idle Timer**: 5-10 seconds (300-600 frames)
- **Animal Wander Speed**: 0.5
- **Animal Movement Range**: 100-750px from Brot
- **Golden Fleece Weight**: 100 coins

## Save System
- **Storage**: localStorage ('chainGameSave')
- **Auto-save**: On coin/item deposit
