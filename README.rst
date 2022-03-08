.. image:: https://zenodo.org/badge/467643820.svg
   :target: https://zenodo.org/badge/latestdoi/467643820
   :align: right

Example for working with the ASpecD framework
=============================================

ASpecD is a Python framework for handling spectroscopic data focussing on reproducibility. In short: Each and every processing step applied to your data will be recorded and can be traced back. Additionally, for each representation of your data (e.g., figures, tables) you can easily follow how the data shown have been processed and where they originate from. For further details, see its `documentation <https://docs.aspecd.de/>`_. A preprint of the publication describing the ASpecD framework is available from ChemRxiv:

* Jara Popp, Till Biskup. ASpecD: A Modular Framework for the Analysis of Spectroscopic Data Focussing on Reproducibility and Good Scientific Practice. *ChemRxiv*, 2021. doi:`10.26434/chemrxiv-2021-6jt1l <https://doi.org/10.26434/chemrxiv-2021-6jt1l>`_.


Aim
---

To provide readers of the publication describing the ASpecD framework with a concrete example of data analysis making use of recipe-driven data analysis, this repository contains both, a recipe (in the file ``example-recipe.yaml``) as well as the UV/vis data that are read, normalised, and plotted.

The actual analysis of the data provided here has been given in:

* Clemens Matt, Deborah L. Meyer, Florian Lombeck, Michael Sommer, Till Biskup. TBT Entirely Dominates the Electronic Structure of the Conjugated Copolymer PCDTBT: Insights from Time-Resolved Electron Paramagnetic Resonance Spectroscopy. *Macromolecules* **52**:4341–4349, 2020. doi:`10.1021/acs.macromol.8b00791 <https://dx.doi.org/10.1021/acs.macromol.8b00791>`_.


Contents
--------

The repository contains four data files, each representing the ASCII export of an optical absorption spectrum of one substance:

* tbt.txt
* cbztbt.txt
* cbztbtcbz.txt
* pcdtbt.txt

The recipe used for recipe-driven data analysis in context of the ASpecD framework resides in:

* example-recipe.yaml


How to analyse the data
-----------------------

In order to analyse the data using the recipe provided, you need to have a working Python installation and the ASpecD framework installed. See the `installation instructions of the ASpecD framework <https://docs.aspecd.de/installing.html>`_ for further details.

Once you have setup everything, performing the analysis from within the directory containing both, data and recipe, is as simple as issuing a single command within a terminal:

  serve example-recipe.yaml

As a result, you should see a file ``uvvis-normalised.pdf`` appear in the same directory, containing the figure representing all four optical absorption spectra normalised each to its low-energy absorption band.


License
-------

All files are licensed under the Creative Commons Attribution-NonCommercial 4.0 International License. See the file ``LICENSE`` for more details.


