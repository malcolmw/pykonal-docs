pykonal.EikonalSolver
=====================

.. toctree::
   :maxdepth: 2
   :caption: Contents:


.. autoclass:: pykonal.EikonalSolver

    +--------------------------------------------------------------------------------------------------+
    |                                       Attributes                                                 |
    +====================+==================+===================+===================+==================+
    |:attr:`close`       |:attr:`coord_sys` |:attr:`iax_null`   |:attr:`is_alive`   |:attr:`is_far`    |
    +--------------------+------------------+-------------------+-------------------+------------------+
    |:attr:`norm`        |:attr:`pgrid`     |:attr:`src_loc`    |:attr:`src_rtp`    |:attr:`src_xyz`   |
    +--------------------+------------------+-------------------+-------------------+------------------+
    |:attr:`uu`          |:attr:`vgrid`     |:attr:`vv`         |:attr:`vvp`        |                  |
    +--------------------+------------------+-------------------+-------------------+------------------+

    +----------------------------------+
    |          Public Methods          | 
    +==================================+
    |:meth:`solve`                     |   
    +----------------------------------+
    |:meth:`trace_ray`                 |   
    +----------------------------------+
    |:meth:`transfer_travel_times_from`|   
    +----------------------------------+
    |:meth:`transfer_velocity_from`    |   
    +----------------------------------+

    .. autoattribute:: close
    .. autoattribute:: coord_sys
    .. autoattribute:: iax_null
    .. autoattribute:: is_alive
    .. autoattribute:: is_far
    .. autoattribute:: norm
    .. autoattribute:: pgrid
    .. autoattribute:: src_loc
    .. autoattribute:: src_rtp
    .. autoattribute:: src_xyz
    .. autoattribute:: uu
    .. autoattribute:: vgrid
    .. autoattribute:: vv
    .. autoattribute:: vvp

    .. automethod:: solve(self)
    .. automethod:: trace_ray(self, end, step_size=None)
    .. automethod:: transfer_travel_times_from(self, old, origin, rotate=False, set_alive=False)
    .. automethod:: transfer_velocity_from(self, old, origin, rotate=False)
