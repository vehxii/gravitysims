# N-body-Gravity-Simulation
Attempting to simulate various gravitating systems, such as galaxies, solar systems, and dark matter halos using a Python n-body gravity simulation.

credit: @pmocz for initial setup --> https://github.com/pmocz/nbody-python/blob/master/nbody.py

<ins>General Process:</ins>
1. Initialize particles (randomly dispersed over a circle, with random masses in a given range). There is fine (but clunky) control over the individual particle masses, locations, initial velocities, etc
2. Get net force on a particle by computing all pairwise interactions between particles
3. Update particles using "leapfrog integration" (kick-move-kick)
4. Save snapshot of simulation to a PNG, then string together all PNGs into a GIF animation once the simulation is done
