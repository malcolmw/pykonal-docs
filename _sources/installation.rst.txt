Installation
============
PyKonal has been tested with Python >=3.7 on Linux (Ubuntu 20.04LTS, 19.10,
18.04LTS) and Mac OS X (10.13) operating systems. It should run on Windows but
is untested.

Installation is via a setup.py file and requires numpy and
Cython to be installed prior to building. `Conda <https://www.anaconda.com>`_
is recommended for managing Python environments and dependencies.  

Dependencies
------------
* cython [>=0.29.14]
* h5py
* numpy


Conda (Recommended)
-------------------
.. code-block::

   sh$> conda create --name pykonal -c conda-forge python=3.8 'cython>=0.29.14' h5py numpy
   sh$> conda activate pykonal
   sh$> cd path/to/pykonal
   sh$> pip install .

pip
---
.. code-block::

   pip install cython>=0.29.14 h5py numpy
   cd path/to/pykonal
   pip install .

