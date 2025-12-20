---
authors:
  - name: null
---

# 3 Metadata and Suggested File Formats

## 3.1 Project Metadata

The metadata elements presented in sections 3.1 to 3.5 can also be be downloaded in a spreadsheet format as [xlsx](../images/CRP-MetadataTemplate.xlsx) or [ods](../images/CRP-MetadataTemplate.ods) files.

```{list-table} Project Metadata
:header-rows: 1

* - Element
  - Description
* - Title
  - The project name or name for the dataset
* - Description
  - The original purpose for the survey work.
* - Subject
  - Keywords for the subject content of the dataset (qualified using e.g. the English Heritage NMR Monument Type Thesaurus or the MDA Object Type Thesaurus.
* - Coverage
  - Site location and description. The address, or coordinates for the site and a description of the site and object or structure to be surveyed. Coverage should also include any relevant period terms.
* - Creators
  - Full name and organization(s) of the surveyor(s)
* - Identifiers
  - Project or reference numbers used to identify the dataset.
* - Dates
  - Date or dates that the survey was conducted in both the field and/or lab.
* - Intended accuracy or scale of the survey
  - The originally intended accuracy or scale that the survey was to achieve. 
* - Description of reference information used
  - Describe any existing reference information available to the surveyor(s), including paper plans or digital spatial data of the site or object. 
* - Additional project notes
  - Any additional project notes that the surveyor feels applicable.
```

## 3.2 Camera Metadata

### 3.2.1 Camera calibration

```{list-table}
:header-rows: 1

* - Element
  - Description
* - Date of calibration
  - Date that the calibration was performed. 
* - Camera calibration file name
  - The exact file name for the camera calibration.
* - Camera specifics
  - Specific make and model of the camera and lens used.
* - Array dimensions in pixels
  - Width and height of digital array measured in pixels.
* - Array dimensions in mm
  - Width and height of digital array measured in millimeters. 
* - Focal length and principal point
  - Exact focal length and principal point location and measured by the camera calibration.
* - Lens distortions (K1, K2, P1 and P2 parameters)
  - Radial and decentering distortion parameters as measured by the camera calibration. 
* - Affine distortions
  - Affine distortion parameters as measured by the camera calibration (if measured). 
* - Calibration Quality Values
  - Quality values such as overall RMS, maximum residual, and photo coverage (%) from the calibration process.
* - Calibration adjustment report
  - A report on the quality of the camera calibration including at a minimum the correlation between exterior and interior parameters
```

### 3.2.2 Calibration images

```{list-table}
:header-rows: 1

* - Entry
  - Description
* - Image file names
  - File names for calibration images. 
* - Calibration target description
  - Include target dimensions, creator and description.
```

## 3.3 Image Metadata

```{list-table}
:header-rows: 1

* - Entry
  - Description
* - __For each group of images__
  - 
* - Project name
  - Same as Project Name in section 3.1.1.
* - Number of images
  - Total number of images submitted for archival. 
* - File name for planimetric sketch or map
  - File name and extension. Should include outline of subject and surrounding objects (if any), indicated location and orientation of each image (using a "V" symbol), and other special comments and/or observations.
* - Camera calibration file
  - Reference to the camera calibration specifics in section 3.2.1.
* - Additional notes
  - Any additional notes the surveyor feels applicable. Could list images containing control and/or scaling references. 
* - __For each image__
  - 
* - Image file name
  - File name and extension.
* - Textural description of location and orientation
  - Should describe general location (e.g. north side) and camera to subject orientation (e.g. view to south). 
* - Format conversions (if any)
  - List of format conversions performed on the digital images and the software used.
```

## 3.4 Reference/datum Metadata

```{list-table}
:header-rows: 1

* - Entry
  - Description
* - __For each control point__
  - 
* - Source and datum (total station, GPS, etc. and WGS84, UTM, LRF)
  - Identify the source for control point collection and the datum used during data collection.
* - xyz coordinates
  - List the three-dimensional coordinates for each control point.
* - xyz covariance matrix
  - Provide full correlation if available (from survey adjustment or GPS baseline solution), otherwise provide estimated standard deviation or variance of each coordinate.
* - Textual description of location
  - Provided a textual description for the location of each control point.
* - Image with control point location indicated
  - An image with the control point location clearly indicated.
* - Geometric constraints on reference features or control
  - List any known geometric constraints for reference features or control.
* - Coordinate System
  - Name of coordinate system, datum and projection.
```

## 3.5 Model Metadata

The following entries could be entered individually or contained within one text file.

```{list-table}
:header-rows: 1

* - Entry
  - Description
* - Name and version of the software
  - Include all details of the software name, manufacturer, and version used.
* - RMSE values
  - Root Mean Square Error (RMSE) for control and check point measurements, indicating whether the RMSE is for control points only, check points only, or all points. 
* - Constraints on object points
  - List of constraints used during processing.
* - __For each point:__
  - 
* - Point type
  - Tie, Control, or Check point.
* - XYZ priori and a priori
  - XYZ coordinates before and after bundle adjustment (control and check points only).
* - Covariance matrix a priori
  - If available, provide the covariance matrix.
* - Image coordinates and residuals
  - A list of images on which the point is indicated. For each image on the list, provide the uv coordinates and residual.  
* - __For each image:__
  - 
* - Exterior orientation
  - List exterior orientation parameters for each image.
```