PointSourceSolver
=================
This example demonstrates how to use the :class:`pykonal.solver.PointSourceSolver` class.

.. code-block:: python

   import numpy as np
   import pykonal
   
   solver = pykonal.solver.PointSourceSolver(coord_sys="spherical")
   
   # Define a simple computational grid.
   solver.velocity.min_coords = 1., 0, 0
   solver.velocity.node_intervals = 1, np.pi/31, np.pi/31
   solver.velocity.npts = 32, 32, 62
   solver.velocity.values = 5 + np.random.rand(*solver.velocity.npts)
   
   # Initialize the source location with a random location within the
   # computational grid.
   delta = solver.velocity.max_coords - solver.velocity.min_coords
   solver.src_loc = np.random.rand(3) * delta + solver.velocity.min_coords
   
   # Compute traveltimes.
   solver.solve()


.. image:: figures/point_source_solver.png
