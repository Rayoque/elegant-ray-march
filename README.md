# Elegant Ray March

A compact, elegant real-time signed distance field (SDF) ray marcher written entirely in WebGL.

**Live Demo:** https://rayoque.github.io/elegant-ray-march

## Features

- Real-time ray marching completely on the GPU
- Multiple materials (matte, chrome, gold, glass)
- Soft shadows + ambient occlusion
- Reflections (up to 3 bounces)
- Smooth camera controls (mouse orbit + WASD movement)
- Two scenes: Classic and Sculpture (with moving elements)
- Simple two-state sidebar with controls
- Fully self-contained single HTML file

## Controls

- **Mouse drag** — Orbit the camera
- **Scroll wheel** — Zoom in/out
- **WASD / Arrow keys** — Move the target (camera-relative)
- **Q / E** — Move up and down
- **Shift** — Faster movement
- **R** — Reset camera

## Running Locally

Just open `index.html` in any modern browser. No build step or dependencies required.

For a better experience, run a local server:

```bash
# Python
python -m http.server 8000

# Then open http://localhost:8000
```

## Technology

- Pure WebGL (no frameworks)
- ~290 lines of GLSL
- All rendering happens in the fragment shader on the GPU

## Development Philosophy

This project is deliberately kept as a **single HTML file** for maximum simplicity and zero build tools. The entire application (UI, controls, and the ray marcher) lives in one file.

## License

MIT

---

Made with curiosity and far too many iterations.