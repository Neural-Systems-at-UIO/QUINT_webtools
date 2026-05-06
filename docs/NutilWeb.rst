**WebNutil**
==============

WebNutil is used to perform the quantification step in the QUINT-online workflow.  It combines the result of the atlas-registration steps (using WebAlign and WebWarp) with the result of the feature extraction step (using Webilastik or another software) to generate a series of reports. These include counts of extracted features and calculates area fraction per reference atlas regions. It also creates point clouds representing the features in 3D atlas space. The results can be downloaded using the "export" button or used interactively in workbench using the plotting Sandbox and MeshView 3D atlas viewer.

**How to open WebNutil?**
-------------------------

.. tip::     
    As WebNutil uses the output of the atlas-registration and feature extraction steps to perform quantification, these steps must be completed before attemping WebNutil analysis.

1. Navigate to WebNutil using the button in your project or using the WebNutil tab at the top of the screen.
 
.. image:: images/WebNutil.png

2. If you have used Webilastik to create segmentations, these will be visible in the middle panel. If you have created your own segmentations using an external software, upload these to WebNutil using the "upload segmentations" button.

3. Once the atlas-registration step is complete and segmentations are available for all your sections (either created with webilastik or uploaded manually), you are ready to perform WebNutil analysis. To do this, select the object colour to quantify in your segmentations in the right hand panel. For segmentations created using Webilastik this is usually "Red" with RGB colour code: 255 0 0. For segmentations created using other software, select the RGB colour code of the objects you wish to quantify.
4. Press "Run Analysis". The results will automatically appear in the results panel when the analysis has completed (this may take some time). 
5. Once WebNutil analysis has completed, download your results, and explore the results interactively using the plotting Sandbox and MeshView atlas viewer. 

.. image:: images/Available_results.png

.. image:: images/Plot.PNG