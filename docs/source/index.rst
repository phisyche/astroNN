.. astroNN documentation master file, created by
   sphinx-quickstart on Thu Dec 21 17:52:45 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. warning:: This is a draft version of astroNN 0.99 Alpha

.. warning:: All plotting functions are currently broken and removed from the master branch, will be fixed this week

Welcome to astroNN's documentation!
======================================

.. toctree::
   :maxdepth: 3
   :caption: Contents:

astroNN is a python package to do various kind of neural networks for astronomers. It provides bayesian neural network
implementation to do neural network with incomplete labeled data and uncertainty analysis. 
Incomplete labeled data means you have some target labels, but you only has a subset of them for some data. astroNN 
will look for -9999. in training data and not backpropagate those particular labels for those particular datas. For 
uncertainty analysis, please see the demonstration section.

As of now, this is a python package developing for an undergraduate research project on deep learning application in 
stellar and galactic astronomy using SDSS APOGEE DR14 and Gaia DR1.

Getting Started
---------------
astroNN is developed on GitHub. You can download astroNN from its Github_.

Recommended method of installation as this python package is still in active development and will update daily:

.. code-block:: bash

   $ python setup.py develop

Or run the following command to install after you open a command line window in the package folder:

.. code-block:: bash

   $ python setup.py install

List of Tutorial
""""""""""""""""""""""""""
* :doc:`/quick_start`
* :doc:`/compile_datasets`
* :doc:`/tools_apogee`
* :doc:`/tools_gaia`
* :doc:`neuralnets/neural_network`

  * :doc:`neuralnets/CNN`
  * :doc:`neuralnets/BCNN`
  * :doc:`neuralnets/Conv_VAE`

* Neural Network Astronomy Paper (Re)Implementation

  * :doc:`neuralnets/StarNet2017`
  * :doc:`neuralnets/GalaxyGan2017`

* :doc:`/history`
* :doc:`/known_issues`

Demonstration
==================
* :doc:`neuralnets/vae_demo`
* `Uncertainty Analysis in Bayesian Deep Learning Demonstration`_

Authors
==================
-  | **Henry Leung** - *Initial work and developer* - henrysky_
   | Astronomy Undergrad, University of Toronto
   | Contact Henry: henryskyleung [at] mail.utoronto.ca

-  | **Jo Bovy** - *Supervisor of Henry Leung* - jobovy_
   | Astronomy Professor, University of Toronto

-  | :doc:`/acknowledgments`

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

.. _Github: https://github.com/henrysky/astroNN
.. _henrysky: https://github.com/henrysky
.. _jobovy: https://github.com/jobovy
.. _Uncertainty Analysis in Bayesian Deep Learning Demonstration: https://github.com/henrysky/astroNN/tree/master/demo_tutorial/NN_uncertainty_analysis