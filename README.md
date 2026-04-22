# Advanced Bouncing Bell Game

A modern, feature-rich browser-based bouncing ball game with advanced gameplay mechanics, visual effects, and power-up systems.

## 🎮 Features

### Core Gameplay
- **Lives System**: Start with 3 lives; lose a life when the ball falls below the paddle
- **Combo Multiplier**: Build combos by hitting bells consecutively without dropping the ball (up to 5x multiplier)
- **Level Progression**: Advance through levels with increasing difficulty
- **Multiple Bells**: More bells appear as you progress through levels
- **High Score**: Persistent high score saved in browser localStorage

### Power-Up System
Random power-ups drop from destroyed bells (20% chance):
- ⚡ **SPEED** - Ball moves 50% faster for 5 seconds
- 🐌 **SLOW** - Ball slows down by 40% for 5 seconds
- 📏 **BIG PADDLE** - Paddle widens by 50% for 8 seconds
- ❤️ **EXTRA LIFE** - Gain an additional life

### Visual Effects
- Modern gradient background with dynamic color themes
- Glowing neon effects on ball, paddle, bells, and power-ups
- Particle explosion system when bells are destroyed
- Ball trail effect showing movement path
- Animated pulsing bells with radial gradients
- Rotating diamond-shaped power-ups
- Floating combo text animations

### Controls
- **Mouse**: Move paddle left/right
- **Touch**: Drag on mobile devices
- **Keyboard**: 
  - `←` / `A` - Move paddle left
  - `→` / `D` - Move paddle right
  - `SPACE` - Pause/Resume game

### User Interface
- Professional start screen with instructions
- Live stats display (score, level, lives, combo, multiplier)
- Active power-up indicators with timers
- Pause overlay with resume/restart options
- Enhanced game over screen with final statistics
- Sound toggle button
- Mobile-responsive design

## 🚀 Getting Started

### Prerequisites
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No installation required!

### How to Play
1. Open `index.html` in your web browser
2. Click "Start Game" or press SPACE to begin
3. Move the paddle to bounce the ball and destroy bells
4. Catch power-ups for special abilities
5. Don't let the ball fall below the paddle!
6. Progress through levels by destroying all bells

### Game Mechanics
- **Scoring**: 
  - Base points per bell: 100
  - Combo bonus: Multiplier × 50 per consecutive hit
  - Level completion bonus: 500 × level number

- **Level Progression**:
  - Level 1: 3 bells
  - Each subsequent level adds 2 more bells
  - Ball speed increases by 5% per level

- **Combo System**:
  - Hit bells consecutively without dropping the ball
  - Combo resets if ball falls below paddle
  - Maximum 5x multiplier at 5+ combo

## 🎨 Customization

You can easily customize the game by editing the `index.html` file:

### Adjust Difficulty
```javascript
// Starting lives
const INITIAL_LIVES = 3;

// Ball speed increase per level (0.05 = 5%)
const SPEED_INCREMENT = 0.05;

// Power-up drop rate (0.2 = 20%)
const POWERUP_DROP_CHANCE = 0.2;
```

### Visual Themes
Modify the gradient colors in the CSS:
```css
body {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

### Power-Up Durations
```javascript
const POWERUP_DURATIONS = {
    speed: 5000,      // 5 seconds
    slow: 5000,       // 5 seconds
    bigPaddle: 8000,  // 8 seconds
};
```

## 📱 Mobile Support

The game is fully responsive and supports touch controls:
- Touch and drag to move the paddle
- Optimized for various screen sizes
- Prevents default touch behaviors for smooth gameplay

## 🔧 Technical Details

### Technologies Used
- HTML5 Canvas for rendering
- Vanilla JavaScript (no frameworks required)
- CSS3 for styling and animations
- Web Audio API for sound effects (optional)
- localStorage for high score persistence

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome Android)

### Performance
- Optimized render loop using `requestAnimationFrame`
- Efficient particle system with object pooling
- Smooth 60 FPS gameplay on modern devices

## 📄 License

This project is open source and available for personal and educational use.

## 🙏 Acknowledgments

Inspired by classic arcade breaker games with modern enhancements.

---

**Enjoy the game!** 🎮✨