# simpleMD
Simple (and incorrect) demonstration of a Molecular Dynamics simulation in Python.

## Overview

I made this when I was in undergraduate at Michigan State University as part of a Honors project for [CMSE 201](https://cmse.msu.edu/academics/undergraduate-program/undergraduate-courses/cmse-201-introduction-to-computational-modeling/). The idea, as prompted, was to demonstrate and visualize a working [Molecular Dynamics](https://en.wikipedia.org/wiki/Molecular_dynamics) (MD) Simulation and then visualize it using [Ovito](https://www.ovito.org/).

`velocity_init.ipynb` uses Python to randomly generate (using a uniform random generation distribution) velocity vectors for a set of N particles. Then `mds.ipynb` uses these vectors to generate M timesteps of simulation, tracking each particles kinetic energy, velocity, and location. Forces are calculated using the [Lennard-Jones Potential](https://en.wikipedia.org/wiki/Lennard-Jones_potential). Boundary conditions are applied (particles simply move to the other side of the box, there is no "bouncing."

If this program was run as is and visualized, it would appear that the particles are unaffected by each other and continue on the path defined by their initial velocity vector. I was never able to solve this problem during the class but I would hazard to guess it is because the geometry of the problem is too large. The Lennard-Jones Potential only appreciably affects particles very close together. I have no expectations of working on this code in the near future, but this serves as a simple demonstration of how to compile an MD simulation using basic Python skills.

All data for the simulation is saved and formatted in a readable format for Ovito.

## Installation

These are Python Jupyter Notebooks that save data in a format useable by Ovito. I have not tested this code recently so it may need minor fixing.

#### Note: I have included my final project presentation from the class as reference material.
