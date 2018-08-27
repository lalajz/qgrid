.. image:: https://media.quantopian.com/logos/open_source/qgrid-logo-03.png
    :target: https://qgrid.readthedocs.io
    :width: 190px
    :align: center
    :alt: qgrid

=====
qgrid
=====
Qgrid is a Jupyter notebook widget which uses `SlickGrid <https://github.com/mleibman/SlickGrid>`_ to render pandas
DataFrames within a Jupyter notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and
filtering controls, as well as edit your DataFrames by double clicking cells.


[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/lalajz/qgrid/master)


API Documentation
-----------------
API documentation is hosted on `readthedocs <http://qgrid.readthedocs.io/en/latest/>`_.

Installation
------------

Installing with pip::

  pip install qgrid
  jupyter nbextension enable --py --sys-prefix qgrid

  # only required if you have not enabled the ipywidgets nbextension yet
  jupyter nbextension enable --py --sys-prefix widgetsnbextension

Installing with conda::

  # only required if you have not added conda-forge to your channels yet
  conda config --add channels conda-forge

  conda install qgrid

Jupyterlab Installation
-----------------------

First, go through the normal installation steps above as you normally would when using qgrid in the notebook.
If you haven't already install jupyterlab and enabled ipywidgets, do that first with the following lines::

  pip install jupyterlab
  jupyter labextension install @jupyter-widgets/jupyterlab-manager

Install the qgrid-jupyterlab extension and enable::

  jupyter labextension install qgrid
