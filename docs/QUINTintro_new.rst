**What is the QUINT workflow?**
===============================
   
The QUINT workflow is an analysis solution for 2D rodent microscopy data, answering the need for brain-wide mapping and regional quantification. The workflow is used to quantify cells and establish maps of cell distribution, receptor densities, connectivity patterns or pathological protein accumulation in the brain. 

.. image:: images/QUINTsummary_2.PNG

.. tip::   
   The `QUINT workflow <https://neural-systems-at-uio.github.io/>`_ is available in the Online Workbench as a suite of web-based tools or offline as downloable tools.

   The Online Workbench offers tighter integration of the tools, shareable viewer links, metadata management and the option to submit directly to `EBRAINS <https://www.ebrains.eu/data/share-data>`_.

Which atlases are supported?
------------------------------

The analysis is performed relative to a reference brain atlas, with the following atlases supported:

1. Allen Mouse Brain Atlas Common Coordinate Framework version 3 (2017) (CCFv3)
2. Waxholm Atlas of the Sprague Dawley rat, version 3 and 4 (WHS rat brain atlas).

.. image:: images/atlases.PNG

What is the output of the tools?
---------------------------------

The workflow generates object counts and area fraction in reference atlas regions, in addition to point clouds that can be used to view the features in 3D with our Meshview Atlas Viewer.  

.. image:: images/results.PNG

How to access the tools?
----------------------------------------

.. Warning:: 
   It is recommended to work in the Google Chrome Browser (not Firefox). This is because some of the tools do not currently work in other browsers.  

1. To access, go to the `Online Workbench <https://ebrains-workbench.apps.hbp.eu/>`_, register for an EBRAINS account and login.
2. You are now ready for the first step in the workflow. `Upload files <https://quint-webtools.readthedocs.io/en/latest/CreateBrain.html>`_. 

