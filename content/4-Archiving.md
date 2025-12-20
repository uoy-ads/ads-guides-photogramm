---
authors:
  - name: null
---

# 4 Archiving Close-range Photogrammetric Data

## 4.1 Preparing to Archive

### 4.1.1 Minimum Files Needed for Archive

At a minimum, any close-range photogrammetry project submitted for archive will consist of a group of raster images and associated metadata (project level details and camera information).

It is recommended that the group of raster images should be accompanied by, at a minimum, three of the metadata groups described in this guide: 1) the Project Metadata, 2) the Camera Metadata, and 3) the Image Metadata. If control points are collected and submitted with the project, the metadata listed in the Reference/datum Metadata must also be included.

If the project is processed using photogrammetric software, and vector products of this further processing (including 2D vector graphics, point clouds, and 3D surface models) are to be archived, metadata according to those file types should be included. Section 3.4 of the [Laser Scanning guide](https://doi.org/10.5284/rt5g-dm24) and Section 4.6 of the [CAD guide](https://doi.org/10.5284/k5hd-hj61) should be used for these.

For raster products, see Section 3 of the [Raster Images guide](https://doi.org/10.5284/mtgj-7130) to learn more about preparing raster images for archive. One important note is to never crop (or change the height/width in any way) an image intended for photogrammetry.

### 4.1.2 File Naming and File Formats

For close-range photogrammetry projects moving further in the processing (especially those creating three-dimensional objects) a range of formats are available depending on the software used. Among the acceptable formats for the submission of two- and three-dimensional objects are ASCII, DXF, OBJ and X3D. See the table below for a more detailed explanation of these formats and when to choose them. 

For a general discussion on file naming, please refer to the general section on [*Planning for the Creation of Digital Data*](https://doi.org/10.5284/h0p2-5584). As a good rule of thumb, file names should be logical and should not contain special characters. In the metadata sections, file names are suggested for each of the interim data sets generated from processing photogrammetric data. For example, it is suggested that all datasets be prefixed by the project name followed by a brief description or shorthand of what the dataset contains. 

__Raster__

The formats described in the table below are recommended for the long-term preservation of digital raster images:

```{list-table}
:header-rows: 1

* - Preservation Format
  - Requirements
* - .tif / .tiff
  - TIFF 6.0 remains widely accepted as a preservation format for digital raster images and includes support for EXIF metadata.
* - .dng
  - As an open extension of the TIFF/EP standard with support for EXIF, IPTC and XMP metadata, the Adobe DNG format is rapidly becoming accepted as a standards for storing raw image data (primarily from digital photography).
```

__Vector__

The formats described in the table below are recommended for the long-term preservation of digital vector graphics:

```{list-table}
:header-rows: 1

* - Format
  - Properties/Technologies
  - Description
  - Recommendations
* - .txt, .csv
  - A simple, text only file used to store textual information in a database table using the ASCII standard code
  - Text files can store data in a database table by delimiting individual pieces of information within a row (or record) with a comma, semi-colon, or space.
  - See Section 3.1 of the [Laser Scanning guide](https://doi.org/10.5284/rt5g-dm24) for more information on this format.  
* - .obj
  - OBJ is an open format storing 3D objects and is accepted by nearly all CAD/3D modeling software
  - OBJ files can be used to store a wide range of 3D objects. OBJ can store files with high polygon counts and polygon textures.
  - See Section 3.1 of the [Laser Scanning guide](https://doi.org/10.5284/rt5g-dm24) for more information on this format. 
* - .x3d
  - X3D was developed for the storing of complex 3D objects and is an ISO standard (ISO/IEC 19775-1.2:2008)
  - X3D is an open format used in a number of open source 3D modeling software packages. Polygonal models stored in X3D can retain textures, normals, and a number of other features used for renderings.
  - This format is an alternative for and similar to the OBJ format. 
* - .dxf
  - An Autodesk AutoCAD file format. Can be opened or created by a large number of other software systems
  - Good for interoperability between CAD and a large number of other software systems, namely GIS software.
  - See Section 3.3 of the [CAD guide](https://doi.org/10.5284/k5hd-hj61) for more information on this format.
```

### 4.1.3 Copyrights

See the section, [Copyright and Intellectual Property Rights (IPR)](https://doi.org/10.5284/h0p2-5584) of the ADS guides for more information on copyrights. 