# Elegant Ray March

A compact, elegant real-time ray marcher built entirely in WebGL using signed distance fields.

**Live Demo:** [https://rayoque.github.io/elegant-ray-march](https://rayoque.github.io/elegant-ray-march)

## Features

- **Pure GPU rendering** — All ray marching and shading happens in the fragment shader
- **291 lines of GLSL** — The entire rendering pipeline is written in a single shader
- Multiple materials with realistic lighting (matte, chrome, gold, glass)
- Soft shadows and ambient occlusion
- Reflections (up to 3 bounces)
- Smooth camera controls (mouse orbit + keyboard movement)
- Two distinct scenes: Classic and Sculpture (with animated elements)
- Responsive sidebar with real-time controls
- Fully self-contained — no build step required

## Controls

| Input              | Action                              |
|--------------------|-------------------------------------|
| Mouse Drag        | Orbit the camera                    |
| Scroll Wheel      | Zoom in/out                         |
| W / A / S / D     | Move camera target (camera-relative)|
| Arrow Keys        | Same as WASD                        |
| Q / E             | Move up / down                      |
| Shift             | Increase movement speed             |
| R                 | Reset camera                        |

## Scenes

- **Classic** — A balanced scene with varied materials and interesting geometry.
- **Sculpture** — Features a central kinetic sculpture with a moving orbiting sphere.

## Running Locally

Open `index.html` in any modern browser. For the best experience, use a local server:

```bash
# Python 3
python -m http.server 8000

# Then open http://localhost:8000
```

## Technology

- Pure WebGL (no external runtime dependencies)
- **291 lines of GLSL** in the fragment shader
- All rendering happens on the GPU
- Intentionally kept as a single HTML file for simplicity

## Development

This project is deliberately maintained as one self-contained HTML file. There are no build tools, bundlers, or separate CSS/JS files. This makes it trivial to host, share, or fork.

If you'd like a split version (separate HTML, CSS, and JS) for easier long-term maintenance, let me know.

## License

MIT License

---

Built with curiosity, iteration, and a healthy disregard for "best practices" in the name of simplicity.