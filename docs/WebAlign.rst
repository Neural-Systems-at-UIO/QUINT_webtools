**WebAlign**
============

WebAlign is a tool for spatial registration of serial section images to a 3D reference brain atlas. Different experimental datasets can be registered to the same reference atlas allowing you to spatially integrate, analyse and navigate the datasets within a standardised coordinate system. 

How to access WebAlign?
------------------------

In "Apps & Analysis", click "WebAlign" and select the brain image series to register to the atlas. Your images will load in the WebAlign app. 

.. image:: images/WebAlign_updated.PNG

How to register my images?
---------------------------

Once a section is registered to the atlas, WebAlign automatically estimates the position of remaining section within the atlas based on the section numbering. It is recommended to register one section in the beginning of the series and one section towards the end of the series as the first step to speed up the registration process. 

1. Select the image in the filmstrip. The main window shows the selected image with the atlas overlay. The colour of the image border reflects registration status (green - registered, orange - in progress, white - not registered).

.. tip:: If necessary, change the cutting plane of the atlas from coronal to sagittal or horizontal view to match the cutting plane of your sections using the dropdown in the Control panel.

2. To register the image, move the cutting plane through the atlas to its approximate position in the atlas using the yellow dots in the sagittal, horizontal and coronal viewer windows (Navigation panel). The main window should now show an atlas overlay that roughly matches your section.

3.  The main window supports mouse drag in multiple modes in order to adjust the atlas overlay to match the outer borders as well as anatomical landmarks within the section (translation and transformations).  

* Markers are positioned using the "Space bar". It is initially a cross and is the fix point of transformations to the atlas overlay. The "Esc key" can be used to remove the marker (in full screen mode the "Esc key" escapes full screen). 
* If there is no marker, or the marker is a cross, mouse drag slides the cut in its plane (translation).
* With a cross in place, press the Up and Down arrows or Left and Right arrows to activate stretch mode. Adjust the atlas overlay to match your section. The panel can be resized towards the left (common border with Control Panel) and towards the bottom (common border with Filmstrip). 

.. note::
  WebAlign performs linear registration only. To refine the registration further use the WebWarp app.

6. Once the image is registered to a satisfactory standard, save the position by pressing "Save". The registration is copied to the remaining slides to help with scaling (visible also in the filmstrip)

7. Go through all the sections, refine the positions and cutting angles and save the registrations.

.. note::
  When jumping from one section to the other, wait a few seconds for the image to load.

.. note::
  The "undo" button allows you to go back to the saved position if necessary.

7. Save your results in a descriptor file (.waln) by pressing "Save".

8. When the registration is finished, export the atlas overlays with the button in the Control panel. 

Short keys
----------------
.. list-table:: 
   :widths: 25 25 50
   :header-rows: 1

   * - **To do this**   
     - **Press**  
     - **Description** 
   * -   Place marker     
     -   Space bar 
     -   Markers are the anchor points of most transformations (stretch and rotate)    
   * -   Remove marker
     -   Esc
     -   Removes a previously placed marker 
   * -   Horizontal stretch from maker 
     -   Left/Right arrow keys 
     -   Marker becomes a vertical line, mouse drag horizontally resizes the cut
   * -   Vertical stretch from maker
     -   Up/Down arrow keys
     -   Marker becomes a horizontal line, mouse drag vertically resizes the cut
   * -   Rotate around marker  
     -   PgUp/PgDown	
     -   Marker becomes a cross with a surrounding arc, mouse drag rotates the cut
   * -   In plane adjust   
     -   Click + drag   
     -   If there is no marker, or the marker is a cross, mouse drag slides the cut in its plane (translation)


Control panel
------------------------
.. list-table:: 
   :widths: 25 50
   :header-rows: 1
   
   * - **Button**   
     - **Function**  
   * -   Store     
     -   Store the current alignment and propagate to unaligned sections (Note this does not save the series to your bucket)
   * -   Restore 
     -   Reset the current alignment to the last stored position
   * -   Clear
     -   Reset the current alignment to the default position
   * -   Overlay Slider
     -   Opacity of the atlas overlay, when fully opaque, it becomes an outline
   * -   Overlay color
     -   The outline color
   * -   Filmstrip slider and color
     -   The above settings, applied to the filmstrip
   * -   Save to bucket
     -   Save the series to your bucket (and overwrite the existing file)
   * -   Export overlays
     -   Generates a series of .flat files (for Nutil or similar utility), and stores them into a .zip file in the bucket (re-using the name of the series descriptor, e.g. series13.json will export series13.zip)
     
.. note:: 
 The right border of the control panel can be dragged horizontally, allowing to resize the panel and the main view

Filmstrip
--------------
Drag horizontally to see series, click on a section in order to load it into the main view. The top border of the filmstrip can be dragged vertically, allowing to resize the panel and the main view

**Navigation panel**
----------------------
Shows the three standard planes centered around the midpoint of the current alignment visible in the main view.

The rectangle of the current cut is projected on each standard plane as a yellow line/rectangle/parallelogram. A small yellow circle represents the midpoint of the projection.

Drag the midpoint around to move the cut.

Drag anywhere else to rotate the cut (inside the given standard plane, around the midpoint)

https://webalign.readthedocs.io/en/latest/
