# ChronoGranular: 150-Bead Hourglass Physics Simulation

A self-contained, single-file HTML5 Canvas 2D granular physics simulation of 150 rigid spheres of varying radii funneling through a rotating hourglass vessel.

- **Live Demo (GitHub Pages):** [https://oik01.github.io/hourglass-sim/](https://oik01.github.io/hourglass-sim/)
- **Source File:** [`index.html`](./index.html)

## Features

- **150 Rigid Spheres of Varying Radii:** Deterministic golden-ratio and linear distribution across `3.8 px` to `7.0 px` (`150` distinct radii) with mass proportional to area ($m = \pi r^2$) and 5 PBR-inspired radial material palettes.
- **Periodic 8-Second Smooth 180° Rotation:** Every `8.0 s`, the hourglass executes a `1.4 s` $C^2$-continuous quintic smoothstep $180^\circ$ rotation (`s(τ) = 6τ⁵ - 15τ⁴ + 10τ³`) with exact rotational wall velocity transfer.
- **Zero-Tunneling & Zero-Overlap Solver:** Combines a $C^1$-continuous analytical local-frame wall profile, 3-step damped Newton-Raphson closest-point projection, 2D elastic and Coulomb frictional impulses, and Symmetric Successive Over-Relaxation (SSOR) positional projection.
- **Interactive Neck Orifice Slider:** Real-time neck width adjustment (`16 px` to `76 px`) with quick presets (`20 px`, `36 px`, `68 px`), manual flip trigger, gravity field control, and live invariant telemetry.
