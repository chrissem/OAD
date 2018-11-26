## Data Tools

Collection of tools that deal with various aspects of image metadata. Some require additional software to create the shwos graphs.

### Batch_Export_OME_TIFF_XML_bfconvert_final.py

* **This tool allows to split and export CZI files to OME-TIFF files.**
* **Has the additional option to create OME-XML files.**
* **It is using the BioFormats command line tools which can be found here:**

[BioFormat Commandline Tools](http://www.openmicroscopy.org/site/support/bio-formats5.5/users/comlinetools/index.html)

***

![Screenshot of GUI](/Images/export_bfconvert1.png)

***

### Display_ZSurface_BF_Python.py

The main idea here is to acquire an image data set and extract the **PlaneData** from the metadata to display those using python tools.
Since python-bioformats does not support the new multi-resolution interface of BioFormats' CZIReader for reading images containing an image pyramid, its is recommend to use BioFormats =< 5.1.10, if the data contains an image pyramid.

***

![Screenshot of ZEN Blue with showing the tool UI](/Images/zsurface_tool1.png)

***

This shows the actual surface of a 96 wellplate, where one position was recorded per well.

***

![2D Z-Surface Plot of Wellplate](/Images/zsurface_tool2.png)

***

Optionally it is possible to also display the surface in 3D.

![3D Z-Surface Plot of Wellplate](/Images/zsurface_tool3.png)

The **PlaneData** can be also saved inside a CSV table.

***

![The PlaneData from the CSV file in Excel](/Images/zsurface_tool4.png)

***

### Metadata_Report_Tool.py

The tools extracts all important metadata and:

* **displays them as a ZenTable directly inside ZEN Blue.**
* **saves it as CSV or TXT file.**
* **opens Excel to fill in the metadata into a sheet.**

![Screenshot of GUI](/Images/MetaData_Report_Tool1.png)

***

### SaveSingeTiles_to_Folder.py

The tools extracts all single tiles from an tile image:

* **select the image to be split from the active documents**
* **specify the desired output folder**
* **select the desired output format for the single tile**

![Screenshot of GUI](/Images/extracttiles.png)