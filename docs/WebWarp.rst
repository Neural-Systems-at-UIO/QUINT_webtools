**WebWarp**
============
WebWarp is a tool for making nonlinear refinements to the atlas registration achieved using WebAlign. Adjustment are applied manually to the atlas overlays by drop and drag of markers placed on the image. 

How to access WebWarp?
----------------------------
In “Apps & Analysis”, click “WebWarp”. Select the image series registered to the atlas using the WebAlign tool. Your images will load in the WebWarp app.

How to make adjustments?
-------------------------

.. image:: images/WebWarp.PNG

1. The sections and corresponding atlas overlays are visible in the Main Window. Adjust the appearance of the atlas overlay with the transparency slider: “Atlas opacity”. The color of the atlas outline can be modified by clicking on the coloured rectangle.
2. To make an adjustment, place a marker on the part of the atlas overlay that you wish to adjust by pressing the space bar. Adjustments are made by dragging the marker using the mouse cursor.
3. To remove a marker, position the mouse cursor over the marker and press Delete or Backspace. 
4. To view the transformations applied, go to “Settings” and “show triangles”. 

.. tip::
 A good strategy is to place markers around the contour of the section first, and then proceed by refining the inner parts.
 
 Try to keep the number of markers to a minimum. 

5. Once you are satisfied with the result, press "Save" and export the atlas overlays with the "Export overlays" button. 

6. You are now ready to extract your features with `WebIlastik <https://quint-webtools.readthedocs.io/en/latest/WebIlastik.html>`_.
 
