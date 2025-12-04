# Game Parameters - Chain Game v0.06

## Canvas
- **Size**: 800x800
- **Background Color**: #000 (black)

## Player
- **Radius**: 12
- **Fill Color**: #000 (black)
- **Outline Color**: #fff (white)
- **Outline Width**: 2
- **Normal Speed**: 3
- **Slow Speed (carrying coin)**: 1.5
- **Acceleration**: 0.3
- **Deceleration**: 0.85
- **Starting Position**: (0, 20)
- **Starting Velocity**: (0, 0)

## Post
- **Base Radius**: 15
- **Dynamic Radius**: Expands to fit coin counter text
- **Color**: #fff (white)
- **Position**: (0, 0) - world center
- **Pulse Alpha Range**: 0.3 - 1.0 (when carrying coin)
- **Pulse Base Speed**: 0.05
- **Pulse Max Speed**: 0.35 (at close proximity)
- **Alpha Return Speed**: 0.1 (interpolation)
- **Coin Counter Display**: Black text centered inside post showing coins needed for next upgrade
- **Coin Counter Font**: bold 24px monospace

## Chain
- **Initial Links**: 5
- **Link Length**: 25
- **Line Width**: 3
- **Line Color**: #888 (gray)
- **Segment Dot Radius**: 3
- **Segment Dot Color**: #aaa (light gray)

## Coins
- **Radius**: 8
- **Color**: #fff (white)
- **Initial Spawn Count**: 100
- **Random Spawn Range**: 150 - 1500 (distance from post)
- **Reachable Coin Min Distance**: maxReach * 0.7
- **Reachable Coin Max Distance**: maxReach * 0.95

## Camera
- **Initial Zoom**: 2.5
- **Minimum Zoom**: 0.5
- **Zoom Interpolation Speed**: 0.05
- **Zoom Reduction Per Chain Extension**: 0.97 (multiply by)
- **Bounce Amount on Coin Deposit**: 0.15
- **Bounce Dampening**: 0.92 (multiply by)
- **Bounce Zoom Multiplier**: 0.3
- **CCC Offset Strength**: 0.5
- **CCC Offset Distance**: 100
- **CCC Offset Interpolation Speed**: 0.08
- **CCC Center Return Speed**: 0.95 (multiply by)
- **Velocity Dampening at Chain Limit**: 0.5 (multiply by)

## Collision
- **Coin Pickup Distance**: player.radius + coin.radius
- **Coin Return Distance**: player.radius + post.radius + 5

## Controls
- **Movement**: Arrow Keys (Up, Down, Left, Right)
- **Fullscreen Toggle**: F key

## Game Logic
- **Coin Stack Offset**: player.radius + 8, plus 12 per additional coin
- **Chain Extension**: +1 link per coin returned
- **Auto-spawn Reachable Coin**: If none exists within reach after coin return
- **Multi-coin Carry**: Enabled (capacity determined by skills)

## Floating Text Effects
- **Text on Coin Deposit**: "+X" where X is number of coins deposited
- **Font**: bold 24px monospace
- **Initial Velocity Y**: -1.5
- **Velocity Dampening**: 0.95 (multiply by)
- **Life Duration**: 1.0 (decreases by 0.015 per frame)
- **Alpha**: Tied to life value
- **Starting Position**: Above post (post.y - post.radius - 10)

## Power-Up System (v0.06)
- **First Power-Up**: 1 coin deposited
- **Threshold Progression**: Fibonacci sequence cumulative (1, 2, 4, 7, 12, 20, 33, 54, 88...)
  - Individual requirements: 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89...
- **Skill Trees**: 4 trees (Up, Down, Left, Right), 25 skills each
- **Progression**: Linear - must take skills in order per tree
- **Menu Style**: High-contrast overlay (85% black), pauses game
- **Selection Delay**: 5 seconds before input is allowed (prevents accidental selection)
- **Countdown Skip**: Each arrow key press reduces countdown by 1 second
- **Countdown Display**: White "[ X ]" brackets with countdown, then "[ READY ]"
- **Selection**: Press arrow key corresponding to desired skill tree
- **Visual Feedback**:
  - Dimmed gray boxes (#555) during delay
  - Bright white boxes (#fff) when selectable
  - Each option in bordered box (220x100px)
  - Arrow symbol, skill name, description, and level displayed per option
  - Description shown in 11px font between name and level

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
