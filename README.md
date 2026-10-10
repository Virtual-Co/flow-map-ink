# Ink Storm

A full-screen living ink painting. Stir procedural marbled art with your finger and watch a real GPU fluid simulation drag it into endless fine filaments that never blur out.

## Run

Open `demo/index.html` in a modern browser with WebGL2. Single file, no build step, no network.

## How it works

A stable-fluids solver (advection, vorticity confinement, pressure projection) drives the flow. A 32-bit backward flow map is advected by that velocity, and the marble pattern is evaluated analytically at each pixel's pulled-back position, so detail is not resampled away. Poured ink is a separate classically advected layer.

## Credit

Technique inspired by the characteristic-mapping idea in Martin Campos Pinto, Victor Fournet, Emmanuel Franck, Philipp Krah and Victor Michel-Dansac, "A neural characteristic mapping method: Lagrangian PINNs based on flow maps for transport-dominated problems", arXiv:2610.12395 (CC BY 4.0). This demo uses the classical flow-map idea only and runs no neural network. No third-party code or assets.

## License

See [LICENSE](LICENSE).
