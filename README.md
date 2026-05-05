# Diamond Atelier — Portfolio Prototype

A protected, pixel-perfect portfolio prototype for the **Diamond Atelier** brand —
a luxury lab-grown diamond showcase featuring cinematic motion design,
animated SVG diamonds, prismatic light effects, and a refined editorial layout.

Live demo (single-file): open `index.html` in a modern browser.

## What's inside

- Single self-contained `index.html` — no build step, no bundler.
- React 18 + Babel runtime (loaded from CDN).
- All custom code, CSS, and component logic is **encrypted** (XOR + base64) and
  decoded at runtime, so the source view does not reveal the design.
- 9 sections: Hero, Trust, Shapes, Colors, Precision, Experience, Collection, Story, Final CTA, Footer.
- Animated SVG diamond with prismatic light streaks.
- Custom cursor, scroll-reveal animations, parallax hero, marquee, hover states.
- Fully responsive (desktop / tablet / mobile breakpoints).

## Protection layer

The build ships with several deterrents that make casual copy/inspection impractical:

- Right-click, drag-start, copy, cut and selection are blocked.
- DevTools shortcuts (`F12`, `Ctrl/Cmd+Shift+I/J/C`, `Ctrl/Cmd+U/S/P/A/C/X`) are intercepted.
- `console.log/debug/info/warn/error/...` are silenced.
- A **DevTools detector** overlays a blocking shield when the inspector is opened.
- The full source (CSS + components) is **XOR-encrypted with base64**, so:
  - View Source shows only a small loader and an opaque payload.
  - There is no separate `.css` file in Network tab — styles are injected at runtime.
  - There is no separate `.js` file — components are decoded into a `text/babel` tag at runtime.
- `noindex / nofollow / noarchive` meta tags discourage search-engine caching.

> Realistic note: client-side code can never be made fully un-copyable —
> a determined developer with a debugger can always unwrap the payload.
> But these layers stop screenshots / view-source / right-click / casual scraping
> and signal that the design is proprietary.

## Credits

Design + build: **Vilol Joshi**.
© 2026 Diamond Atelier prototype. All rights reserved.
