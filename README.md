# Sacred Geometry Reactor — 1

An experimental, browser-based 3D energy-core visualization built with **Three.js**, custom shader materials, bloom post-processing, and a futuristic HUD. The Advanced Edition adds a boot sequence, extra orbital geometry, an expanding energy shockwave, interactive ambient synth audio, and motion/camera controls.

**Developer:** MD.Atiqul Islam (Atik)  
**Email:** [atik.cmttiu1001@gmail.com](mailto:atik.cmttiu1001@gmail.com)

## Features

- **Real-time 3D geometry** — layered sacred-geometry structures, orbiting energy nodes, particles, rings, and a central reactor core.
- **Advanced orbital lattice** — animated procedural torus-knot structures surrounding the reactor.
- **Energy surge** — trigger a one-shot expanding shockwave and temporary bloom/lighting boost.
- **Interactive synth ambience** — optional low-frequency ambient sound generated in-browser with the Web Audio API. Audio starts only after the user clicks the sound control.
- **Futuristic loading screen** — animated startup emblem, progress bar, and system initialization messages.
- **Post-processing** — Unreal Bloom for neon glow and ACES filmic tone mapping.
- **Interactive controls** — toggle audio and automatic motion, trigger an energy surge, and reset the camera.
- **Responsive HUD** — adapts the control deck for smaller screens.
- **No build step** — a single HTML file; Three.js is loaded from a CDN.

## Run locally

Because the project uses JavaScript modules and imports Three.js from a CDN, run it from a local web server rather than opening the file directly.

### Option A — Python

```bash
python -m http.server 8000
```

Then open [http://localhost:8000/Sacred_Geometry_Reactor_Atik_Advanced.html](http://localhost:8000/Sacred_Geometry_Reactor_Atik_Advanced.html).

### Option B — VS Code

1. Open the project folder in VS Code.
2. Install the **Live Server** extension if you do not already have it.
3. Right-click the HTML file and choose **Open with Live Server**.

## Controls

| Control | Action |
| --- | --- |
| Drag | Rotate the 3D scene |
| Scroll / pinch | Zoom |
| **Sound: Off / On** | Toggle generated ambient synth audio |
| **Energy Surge** | Trigger the expanding energy wave |
| **Motion: On / Off** | Toggle automatic camera rotation |
| **Reset View** | Return the camera to its initial position |

## Tech stack

- HTML5 and CSS3
- JavaScript ES modules
- [Three.js](https://threejs.org/)
- Three.js `OrbitControls`
- `EffectComposer`, `UnrealBloomPass`, and `OutputPass`
- Web Audio API
- Google Fonts (Orbitron)

## Project structure

```text
Sacred-Geometry-Reactor/
├── Sacred_Geometry_Reactor_Atik_Advanced.html
└── README.md
```

## Browser and performance notes

- Use a modern browser with WebGL support.
- An internet connection is required for the CDN-hosted Three.js modules and Google Fonts.
- The sound control must be enabled by the user; browsers generally block audio autoplay.
- Bloom and high-DPI rendering can be GPU-intensive. Close other GPU-heavy tabs or use a lower display resolution if performance is poor.
- The experience is an artistic visualization, not a scientific simulation.

## GitHub deployment

1. Create a **public** GitHub repository (for example, `sacred-geometry-reactor`).
2. Add the HTML file and this README.
3. Commit and push your files.
4. To publish with GitHub Pages, open **Settings → Pages**, select the branch and folder containing the HTML file, then save.
5. If GitHub Pages serves the project at the repository root, rename the HTML file to `index.html` for the page to load automatically.

## License

No license has been specified. Add a license file before redistributing or reusing this project if you want to define explicit reuse terms.
