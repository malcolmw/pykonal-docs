Spherical 2D (Polar coordinates)
================================
This example demonstrates the trivial case of a point source at
:math:`(\rho, \phi) = (0, 0)` in a homogeneous velocity model where
:math:`v(\rho, \phi) = 1` [km/s] using a 8 x 8 spherical computational grid. To
get the 2D case in spherical coordinates, we set :math:`\theta=\frac{\pi}{2}`

.. code-block:: python

   import numpy as np
   import pykonal

   # Initialize the solver using a spherical coordinate system.
   solver = pykonal.EikonalSolver(coord_sys="spherical")
   # There is a singularity in the gradient operator at rho = 0, so we can't
   # put a node there. We are fixing theta = pi/2 so that our grid lies in the
   # xy-plane.
   solver.velocity.min_coords = 1, np.pi/2, 0
   solver.velocity.node_intervals = 1, 1, np.pi/8
   # This time we want a 3D computational grid, so set the number of grid nodes
   # in the z direction to 8 as well.
   solver.velocity.npts = 8, 8, 8
   solver.velocity.values = np.ones(solver.velocity.npts)

   # Initialize the source.
   src_idx = 0, 0, 0
   solver.traveltime.values[src_idx] = 0
   solver.unknown[src_idx] = False
   solver.trial.push(*src_idx)

   # Solve the system.
   solver.solve()
