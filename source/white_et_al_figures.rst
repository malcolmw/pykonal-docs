Figures from White et al. (2020)
================================

The Jupyter Notebooks here can be used to reproduce the figures from White et
al. (2020). These notebooks are guaranteed to work with PyKonal version 0.2a0.

Dependencies
------------
These notebooks have additional dependencies:

* jupyter/jupyterlab
* scipy
* matplotlib
* ipympl

The ipympl dependency can easily by alleviated by replacing the first line in
each notebook with a call to your matplotlib backend of choice.

The easiest way to build a working environment is via `Conda <https://www.anaconda.com>`_:

.. code-block::

   conda create --name pykonal -c conda-forge python=3.7 numpy scipy 'cython>=0.29.14' matplotlib ipympl nodejs jupyterlab
   conda activate pykonal
   jupyter labextension install @jupyter-widgets/jupyterlab-manager
   jupyter labextension install jupyter-matplotlib
   cd path/to/pykonal
   python setup.py install

Download
--------
* :download:`figure_3.ipynb <white_et_al_figures/figure_3.ipynb>`
* :download:`figure_4.ipynb <white_et_al_figures/figure_4.ipynb>`
* :download:`figure_5.ipynb <white_et_al_figures/figure_5.ipynb>`
* :download:`figure_6.ipynb <white_et_al_figures/figure_6.ipynb>`
* :download:`figure_7.ipynb <white_et_al_figures/figure_7.ipynb>`
* :download:`figure_8.ipynb <white_et_al_figures/figure_8.ipynb>`

Figure 3
--------
.. image:: figures/jupyter/figure_3.png
   :align: center

Figure 4
--------
.. image:: figures/jupyter/figure_4.png
   :align: center

Figure 5
--------
.. image:: figures/jupyter/figure_5.png
   :align: center

Figure 6
--------
.. image:: figures/jupyter/figure_6.png
   :align: center

Figure 7
--------
.. image:: figures/jupyter/figure_7.png
   :align: center

Figure 8
--------
.. image:: figures/jupyter/figure_8.png
   :align: center
