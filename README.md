# Particle Mesh Gravity Simulation (ENZO-like)
Simple particle-mesh simulation (collisionless "dark matter" only), complete with a density map and GIF animation rendering functionality.

<ins>General Process:</ins>
1. Initialize particles on an even grid (cube)
2. Generate and apply Gaussian random noise in Fourier space
3. Apply Zel'dovich displacements
4. Compute gravitational interactions via solving Poisson's equation in Fourier space (using cloud-in-cell to track the density)
5. Leapfrog integration to move the particles (kick-move-kick technique)
6. Render simulation snapshot to a PNG, then string together the PNGs into a GIF when the simulation is done

Still working on producing stable physical structures like filaments and halos... 
