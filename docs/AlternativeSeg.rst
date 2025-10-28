**Upload your own segmentations**
===================================

The webilastik application in the online workbench can be used to identify the features in the images to quantify using the QUINT online workflow. Alternatively, you can create your own segmentations identifying the features to quantify using any image analysis software (e.g. FIJI, QuPath, Cellpose, ilastik). These can then be uploaded to the online workbench directly in the WebNutil application. 

Any image analysis software may be used to generate the segmentations as long as the segmented images meet the QUINT online requirements.

**Segmentation requirements**
------------------------------

* Format: Must be in PNG format, with the objects to quantify displayed in one RGB colour (e.g. red = 255, 0, 0).

* File naming: the segmentations must have identical file names to the original images uploaded to the workbench. They must comply with the `QUINT file naming convention <https://quint-webtools.readthedocs.io/en/latest/Requirements.html>`_.

* Image proportions: Must have the same proportions as the images uploaded to the online workbench, but are usually not the same size as the original images. It is recommended to downscale the images prior to segmentation using a consistent scaling factor for the whole image series. This has several advantages: it can improve the quality of segmentation as it removes noise from the images. It speeds up WebNutil analysis and can prevent crashes due to insufficient memory. 

.. tip::

    The aim is to downscale the images as much as possible but without losing the information from the images that is actually important. The optimal scaling factor is determined by trial and error and must be applied consistenty to all the images in the image series. 

* Image size: We recommend using segmentations up to a maximum size of 14000 x 10000 pixels. Images larger than this may also work. However, risk of crashing due to insufficient memory increases. It is recommended to downscale the images as much as possible before segmenting them.

.. tip::

    `QuPath: <https://qupath.github.io/QuPath>`_ is an alternative that can be used to generate the segmentations. In some cases QuPath may perform better than ilastik. See `this iprotocol <https://www.protocols.io/view/quint-workflow-for-fluorescence-4r3l22y6jl1y/v2>`_ for how to use QuPath for the QUINT workflow.

    `FIJI: <https://imagej.net/software/fiji/> is also useful for generating segmentations. 





 