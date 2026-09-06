# pour.

**the zen of pouring a glass of water. gen z edition. dopamine included. no cap.**

### ▶ Play now: **https://lethalnoah.github.io/pour/**

Works in any browser. On a phone, add it to your home screen and it runs full screen and offline like a real app.

---

## What is this

A one-button game about pouring a glass of water. Hold to pour, let go at the line. That's it.

The catch: the water still in the air keeps landing after you let go, so the whole skill is learning to release a beat early. Nail it and the game explodes. Miss and it sends you back to the dark.

It is calm until it isn't:

- **Zen layer.** A low ambient drone, a slow breathing glow, a real-physics pour sound whose pitch rises as the glass fills, and a spring-simulated water surface that ripples under the stream.
- **Dopamine layer.** Perfect pours trigger hitstop, screen shake, confetti, chimes, and popups like *NO CAP. PERFECT.* and *IT'S GIVING HYDRATION.* Overflow gets you *COOKED 💀* and the womp-womp.

## How it plays

| do this | get this |
|---|---|
| hold (tap / space) | the tumbler tilts and pours |
| release | the stream cuts, the last of it lands, the glass is judged |
| hit the line | PERFECT, great, good, miss, or overflow |
| chain hits | combo climbs, aura multiplies |
| miss or spill | combo resets, the lights go out |

**Aura** is the score and the currency. Everything you earn comes from actually pouring. There is no idle income.

## The ladder

Your combo drives the whole atmosphere. Every threshold lifts the palette and opens up the music, from *npc mode 🌑* at zero through *flow state 🌊*, *ascending 🔮*, *enlightened fr ☀️*, all the way to *you are the water 💧* at x100. Lose the combo and everything collapses back to the dark drone.

Hit **x100** and you **prestige**: a permanent rank and a permanent aura bonus, plus a golden **halo** that doubles your aura until the next loss.

## Progression

- **Upgrades.** Nine pathways with exponential costs that compound into each other: hydration, combo engine, steady hands, redemption, ignition, challenge master, surface tension, spill shield, and halo. Higher pathways unlock through earlier ones or through feats like a x10 combo. Every pathway has a visible effect on the glass.
- **Challenges.** Random modifiers once you're on a streak: shot glass, big gulp, speedrun, blackout (the water is invisible, judge by pitch), drunk (the line drifts), fanum tax (someone sips your water), and more. Each pays a bonus multiplier.
- **Style.** Cosmetic glasses, water effects that stack, pourer skins, and confetti styles. Priced like monuments. You won't get there without the upgrade tree.
- **Openers and comebacks.** The first glass of a run sets you at x5 on a perfect. A perfect right after a loss is a full comeback moment with its own bonus.

## Install as an app

- **Android:** open the link in Chrome and accept the install prompt, or use *Add to Home screen* from the menu.
- **iPhone:** open the link in Safari, tap **Share**, then **Add to Home Screen**.

Once installed it works offline. Updates arrive automatically the next time you open it, and the game shows a *new version ready* toast when one is waiting.

## Tech

One HTML file, no framework, no build step. Canvas 2D for the scene, Web Audio for every sound (nothing is a sample; the drone, the pour, the chimes, and the slurp are all synthesized), CSS for the popups, `localStorage` for saves, and a small service worker for offline and updates.

### Running locally

Open `index.html` in a browser. For the service worker you need http, so any static server works:

```bash
python -m http.server 8765
```

### Shipping an update

1. Bump `VERSION` in `index.html` (near the top of the script) and in `sw.js`.
2. Commit and push to `main`. GitHub Pages rebuilds in about a minute.

Players get the update toast on their next launch.

## Status

Playable and actively being tuned. The economy, the challenge list, and the visual effects are all still moving. Feedback and combo screenshots welcome.
