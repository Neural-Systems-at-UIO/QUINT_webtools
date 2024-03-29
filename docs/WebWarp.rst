**WebWarp**
============
WebWarp is a tool for making nonlinear refinements to the atlas registration achieved using WebAlign. Adjustment to the atlas overlays are applied manually by dropping and dragging markers. 

.. Warning:: 
WebWarp currently only works in the Google Chrome browser (not Firefox). 

How to access WebWarp?
----------------------------
In “Apps & Analysis”, click “WebWarp”. Select an image series that has already been registered to the atlas using the WebAlign app. Your images will load in the WebWarp app.

How to make adjustments?
-------------------------

.. image:: images/WebWarp.PNG

1. The sections are visible in the Main Window with atlas overlays achieved using WebAlign. Switch between different versions of the atlas overlay using the transparency slider: “Atlas opacity”. The color of the atlas outline can be modified by clicking on the coloured rectangle.
2. To make an adjustment to the atlas overlay, place a marker on the part of the atlas that you wish to adjust by pressing the space bar. Adjustments are made by dragging the marker using the mouse cursor.
3. To remove a marker, position the mouse cursor over the marker and press Delete or Backspace. 
4. Markers can also be used as anchor points, fixing in place parts of the registration that are correct. 
4. To view the transformations applied, go to “Settings” and “show triangles”. 

.. tip::
 A good strategy is to place markers around the contour of the section first (use them as anchors), and then proceed by refining the inner parts.
 
 Try to keep the number of markers to a minimum. 

5. Once you are satisfied with the result, press "Save". Export the atlas overlays with the "Export overlays" button. 

6. You are now ready for the second step of the workflow: extract your features with `WebIlastik <https://quint-webtools.readthedocs.io/en/latest/WebIlastik.html>`_.
 
