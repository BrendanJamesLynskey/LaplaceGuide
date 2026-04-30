# The Laplace Transform — A Graphical Guide

An interactive, animated visual guide to the Laplace Transform, built with vanilla HTML, CSS, and Canvas. Designed for engineering students, self-learners, and anyone who wants to build geometric intuition for one of the most important tools in applied mathematics.

**[→ View the live guide](https://brendanjameslynskey.github.io/LaplaceGuide/)**

---

## What's Inside

The guide walks through eight sections, each with interactive animations you can control in real time:

| Section | What It Covers | Interactive Elements |
|---|---|---|
| **Intuition** | What the transform actually does — decomposing a signal into complex exponentials | σ/ω sliders, animated integration sweep |
| **The Kernel** | Anatomy of e⁻ˢᵗ as envelope × oscillation | σ/ω sliders, phase-animated phasor |
| **The s-Plane** | Poles, zeros, and stability regions | Four presets with animated impulse responses |
| **Sign Reversal** | Why right-half-plane poles are unstable — the minus sign in e⁻ˢᵗ, the system's growth rate, and how they combine inside the integral | — |
| **Common Pairs** | Reference table of essential transform pairs | — |
| **Key Properties** | Linearity, differentiation, convolution, initial/final value theorems | — |
| **Solving ODEs** | Damped spring–mass system response | Damping ratio ζ and natural frequency ωₙ sliders |
| **Region of Convergence** | How the same F(s) with different ROCs gives different time signals | Causal / anti-causal / two-sided presets |



## Tech Stack

Everything is self-contained in a single `index.html` file:

- **HTML5 Canvas** for all animations and plots (no chart libraries)
- **CSS** with custom properties, keyframe animations, and scroll-triggered reveals
- **Vanilla JavaScript** — zero framework dependencies
- **Google Fonts** (Playfair Display, DM Sans, Source Code Pro) loaded via CDN

No build tools, no npm, no bundler. Just open the file.

## Browser Support

Tested on current versions of Chrome, Firefox, Safari, and Edge. Requires a browser that supports ES6, Canvas 2D, and `IntersectionObserver`.

## Customisation

The colour palette and typography are controlled by CSS custom properties at the top of the `<style>` block:

```css
:root {
  --bg: #0a0c10;
  --accent: #4ecdc4;
  --accent2: #ff6b6b;
  --accent3: #ffe66d;
  --accent4: #a78bfa;
  --text: #e2e8f0;
  /* ... */
}
```

Swap these values to re-theme the entire guide.

## License

MIT — use it, remix it, teach with it.
