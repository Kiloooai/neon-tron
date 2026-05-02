# 🌟 Neon Tron

*Light cycle survival game. Ride your neon bike, leave a permanent glowing trail. Avoid walls and your own path. Collect energy orbs to grow and score. Speed increases over time.*

---

## What is this?

A Tron-inspired light cycle game. You control a glowing bike that leaves a permanent light trail behind it. The trail becomes a wall — crash into it or any arena wall and you're done. Collect yellow energy orbs to grow your trail longer and increase your score. The bike speeds up gradually as you collect more orbs. Survive as long as you can. Classic arcade survival, neon-styled.

---

## Features

- **Light cycle mechanics** — bike leaves a permanent glowing trail
- **Collision detection** — hitting walls or your own trail ends the game
- **Energy orbs** — collect them to grow longer and score (+10 each)
- **Progressive speed** — bike gets faster as you collect more orbs
- **Neon aesthetic** — cyan trail, magenta bike, yellow orbs, all glowing
- **Score & high score** — high score saved to localStorage
- **Controls:** Arrow keys or WASD
- **Mobile support** — on-screen D-pad for touch devices
- **Pause/Resume** — Space bar or button
- **Single HTML file** — no dependencies

---

## How to Play

1. Open `index.html`
2. Press **Start** or hit Space
3. Use arrow keys (or WASD) to steer your bike
4. Avoid hitting:
   - The arena walls (edges)
   - Any part of your own light trail
5. Collect glowing yellow orbs to:
   - Increase your score (+10)
   - Grow your trail (harder to avoid)
   - Slightly increase your speed
6. Survive as long as possible
7. Try to beat your high score

**Mobile:** Use the on-screen D-pad that appears at the bottom.

---

## Technical Notes

- Grid-based movement (10px grid on 800×600 canvas)
- Trail stored as array of `{x, y}` coordinates
- Bike speed increases: base 5 grid cells per move, +0.5 per 50 points
- Movement uses accumulator pattern for consistent speed across frame rates
- `requestAnimationFrame` loop with delta-time
- High score saved to `localStorage` under key `neonTronHighScore`
- Collision: simple coordinate equality checks
- Orbs spawn randomly avoiding trail and bike position
- Visuals: stroke for trail (cyan glow), rect for bike (magenta), arc for orbs (yellow)

---

## The Real Story

Tron light cycles are iconic: the wall of light that follows you, the tension of navigating in ever-shrinking space. This captures that essence in a minimal package. The neon glow gives it that cyberpunk future vibe. The increasing speed creates genuine panic. It's the perfect "one more try" game — you always feel you could have done better.

Also: the trail is permanent until death. No fading. That means your mistakes literally follow you.

---

*Made with ✨ and some serious light-cycle energy during a heartbeat build cycle.*

**Repo:** https://github.com/Kiloooai/neon-tron
