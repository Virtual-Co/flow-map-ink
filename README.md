# Ink Storm

An offline, single-file WebGL2 experiment inspired by the flow-map representation in [arXiv:2610.12395](https://arxiv.org/abs/2610.12395). It fuses characteristic-map pullback with a hands-on fluid-art comparison: ordinary repeated dye advection is shown beside a backward map transported through the same live velocity field.

The paper's method learns maps with Lagrangian physics-informed neural networks and composes short learned maps. This demo does not train or run a neural network, does not reproduce the paper's experiments, and instead shows a classical, shader-based characteristic-map idea in a simplified analytic incompressible flow. The velocity is procedural; it is not a pressure-projected stable-fluids solver.

## Run

Open `demo/index.html` in a modern browser with WebGL2 enabled. No build step, server, external assets, or network connection is required.

## Controls

- Drag to stir the field; grab the center divider to reposition it.
- Double-tap / double-click to add a strong local vortex impulse.
- Reset the simulation, cycle three patterns, or switch between split and full view with the buttons.

## Credits and third-party code

Inspired by Martin Campos Pinto, Victor Fournet, Emmanuel Franck, Philipp Krah, and Victor Michel-Dansac, “A neural characteristic mapping method: Lagrangian PINNs based on flow maps for transport-dominated problems,” arXiv:2610.12395 (2026), licensed CC BY 4.0. This demo is an independent implementation of a simplified classical flow-map visualization. It uses no third-party code or external assets.

## License

See [LICENSE](LICENSE).
