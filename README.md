# Team99

Portfolio site for **Team99** — a three-member student developer team from Gyan Ganga
Institute of Technology & Sciences (GGITS), Jabalpur, studying IoT & Cyber Security
(including Blockchain Technology).

We build websites, apps and AI-hardware projects — including a Smart AI-Based Attendance
System that recognises faces in real time on low-cost hardware.

## The site

A single-page portfolio with a scroll-driven "flight" interface. The page itself doesn't
scroll: scroll input drives a camera through a starfield, and each section sits at its own
station in depth, flying toward the viewer as you travel.

- **Canvas starfield** — depth-projected stars and bokeh, with warp streaks when you move fast
- **Nine stations** — Intro, Pitch, Skills, The Stack, Team, Projects, Next, Join Us, Contact
- **Keyword constellation** — the tech stack scattered through 3D space at varying depths

## Tech

Vanilla HTML, CSS and JavaScript. **No build step, no dependencies, no framework.**

```
index.html    markup and content
style.css     styling, layout, flight-mode rules
script.js     starfield engine, camera, flight controller
assets/       team photos
```

## Running locally

Any static file server works:

```bash
python -m http.server 8080
```

Then open <http://localhost:8080>.

Opening `index.html` directly from the filesystem also works.

## Accessibility & fallbacks

The flight interface is progressive, not required:

- **Phones, small windows, and short viewports** fall back to normal document scrolling with
  standard scroll-reveal animations — touch-based scroll hijacking is avoided deliberately.
- **`prefers-reduced-motion`** disables the starfield loop, the fly-in transitions, the ticker
  and the grain overlay.
- Full keyboard navigation in flight mode: arrows, space, Page Up/Down, Home and End.
- Rendering quality adapts automatically — the star field thins and the depth-of-field blur
  drops on machines that can't hold frame rate.

## Team

| | |
|---|---|
| **Akshat Singh Baghel** | Founder & Full Stack Developer |
| **Mohammad Naved** | Co-Founder & Backend Developer |
| **Aryan Vishwakarma** | Co-Founder & UI/UX Developer |

## Contact

<support@team99.tech>

## License

GPL-3.0 — see [LICENSE](LICENSE).
