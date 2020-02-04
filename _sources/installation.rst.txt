Installation
============
PyKonal has been tested with Python 3.7 on Linux (Ubuntu 19.10, 18.04LTS) and Mac OS X (10.13) operating systems. It is not guaranteed to run on Windows.

Installation is via a setup.py file and requires both dependencies (numpy and Cython) to be installed prior to building.

Dependencies
------------
* numpy
* cython [>=0.29.14]


Conda (Recommended)
-------------------
.. code-block::

   conda create --name pykonal python=3.7, numpy, cython>=0.29.14
   conda activate pykonal
   python setup.py install

pip
---
.. code-block::

   pip install numpy cython>=0.29.14
   python setup.py install

