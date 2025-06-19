# AirPods Pro — Scroll Animation

A buttery-smooth, scroll-driven animation that renders 65 sequential frames of AirPods Pro on an HTML canvas as you scroll, inspired by [apple.com](https://www.apple.com/airpods-pro/).

![Astro](https://img.shields.io/badge/Astro-5.9-BC52EE?logo=astro&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-3.13-88CE02?logo=greensock&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1-06B6D4?logo=tailwindcss&logoColor=white)
[![Deploy](https://img.shields.io/badge/Vercel-Live-000?logo=vercel&logoColor=white)](https://airpods-three.vercel.app/)

## Demo

**[airpods-three.vercel.app](https://airpods-three.vercel.app/)**

## Tech Stack

| Layer      | Technology                                       |
| ---------- | ------------------------------------------------ |
| Framework  | [Astro](https://astro.build/) (SSG)              |
| Animation  | [GSAP](https://gsap.com/) + ScrollTrigger        |
| Styling    | [Tailwind CSS](https://tailwindcss.com/) v4      |
| Rendering  | HTML Canvas API                                  |
| Hosting    | [Vercel](https://vercel.com/)                    |

## How It Works

1. **65 PNG frames** are preloaded from Apple's CDN.
2. **GSAP ScrollTrigger** maps scroll progress (0 - 100 %) to a frame index.
3. On every scroll tick the matching frame is drawn to an HTML `<canvas>`, creating the illusion of a 3D product rotation synced to the user's scroll.

## Getting Started

```bash
# Clone
git clone https://github.com/davillafer/airpods.git
cd airpods

# Install dependencies
pnpm install

# Start dev server (localhost:4321)
pnpm dev

# Production build
pnpm build
```

