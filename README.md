# glsl_touchdesigner

A collection of audio-reactive GLSL shader visualizers built in TouchDesigner. Each subdirectory contains a self-contained `.toe` project file. Most shaders are raymarched or simulation-based, designed for real-time audio reactivity and live performance.

---

## Projects

### abstract_vortex
`abstract_vortex/abstract_vortex.toe`

Volumetric raymarched tunnel with rotating turbulence and glowing fog. Uses noise-based wall distortion and ACES tonemapping. The tunnel spirals and warps dynamically. Shader source: `abstract_vortex/volumetric_tunnel.glsl`.

---

### crystal_lattice
`crystal_lattice/crystal_lattice.toe`

Raymarched crystal lattice structure. Shader embedded in `.toe`.

---

### crystalline_swirl
`crystalline_swirl/crystalline_swirl.toe`

Raymarched crystalline sphere with domain distortion creating swirling, folded geometry. Produces radial band patterns, a glowing sun-hit highlight offset from center, and edge color rotation with `tanh` tonemapping. Shader source: `crystalline_swirl/crystalline_swirl.glsl`.

---

### devil
`devil/devil_glass.toe`

Devil glass effect. Shader embedded in `.toe`.

---

### dispersion_sphere
`dispersion_sphere/dispersion_sphere.toe`

Sphere with dispersion/chromatic separation effect. Shader embedded in `.toe`.

---

### foggy_glass
`foggy_glass/foggy_glass.toe`

Foggy glass material effect. Shader embedded in `.toe`.

---

### fractal_volumetric
`fractal_volumetric/fractal_volumetric.toe`

Volumetric fractal renderer using a scaled inverse Mandelbrot-like iteration. Flies forward through a fractal landscape with 50–150 raymarch steps and 8–16 fractal iterations per ray. Supports HSV and RGB color modes with log-based depth coloring. Shader source: `Fractal 2/fractal_volumetric.glsl`.

---

### germarium
`germarium/germarium.toe`

Organic cellular/germarium structure. Shader embedded in `.toe`.

---

### glitch
`glitch/Glitch.toe`

Glitch effect visualizer. Shader embedded in `.toe`.

---

### holodice_tunnel
`holodice_tunnel/holodice_tunnel.toe`

Forward-moving gyroid tunnel with holographic iridescent foil surfaces. Two-layer gyroid frequency patterns, procedural sparkles using voxel-grid hashing, chromatic aberration for iridescent color separation, and sine-wave surface detail. Shader source: `holodice_tunnel/holofoil_tunnel.glsl`.

---

### holofoil_dice
`holofoil_dice/holofoil_dice.toe`

Raymarched chamfered cube (dice shape) with holographic trading card foil effects. Gyroid-based shimmer patterns, procedural sparkles, triple-pass chromatic aberration across RGB channels, and auto-rotating or mouse-interactive view. Shader source: `holofoil_dice 2/holofoil_dice.glsl`.

---

### jello_grid
`jello_grid/jello_grid.toe`

Jello grid simulation/effect. Shader embedded in `.toe`.

---

### kaleidoscope
`kaleidoscope/kaleidoscope_crystal.toe`

Kaleidoscopic crystal pattern generator. Shader embedded in `.toe`.

---

### neon_crystal
`neon_crystal/neon_crystal.toe`

Neon crystal effect. Shader embedded in `.toe`.

---

### physarum
`physarum/physarum.toe`

Multi-pass simulation of *Physarum polycephalum* (slime mold) behavior. Agents perform chemotaxis — sensing chemical trails in three directions and turning toward the strongest signal. Trail map undergoes diffusion (3×3 mean filter) and decay each frame, producing organic branching network patterns. Supports food source attractors/repellers, multiple visualization color modes (grayscale, heat map, HSV, custom gradients), and audio reactivity. Shader sources: `physarum/physarum/`, `physarum/physarum_advanced/`.

---

### radial_creation
`radial_creation/creation.toe`

Radial generative pattern. Shader embedded in `.toe`.

---

### simplex_tunnel
`simplex_tunnel/simplex.toe`

Simplex noise tunnel flythrough. Shader embedded in `.toe`.

---

### the_screen
`the_screen/the_screen.toe`

CRT/LCD screen simulation with bokeh depth-of-field blur, perspective distortion, RGB subpixel patterns, scrolling horizontal text bars with noise variation, and cubic bloom. Produces a nostalgic monitor aesthetic. Shader source: `the_screen/the_screen.glsl`.

---

### volumetric_fractal
`volumetric_fractal/volumetric_fractal.toe`

Enhanced volumetric fractal with animated breathing/pulsing bounds driven by a sine wave. The fractal structure expands and contracts rhythmically, creating a "living" feel. Rotates on the ZY plane (vs. XZ in `fractal_volumetric`). Shader source: `volumetric_fractal/fractal_volumetric_v2.glsl`.

---

## Notes

- Projects without a listed shader source have GLSL embedded directly in the TouchDesigner `.toe` file.
- Original working files are the unnumbered `.toe` files; numbered variants (e.g. `.3.toe`, `.6.toe`) are iteration backups and live in the source `td_shaders/` directory.
- All projects are designed for audio reactivity — parameter mappings vary per project and are configured inside each `.toe`.
