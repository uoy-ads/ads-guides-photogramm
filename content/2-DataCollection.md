---
authors:
  - name: null
---

# 2 Data Collection and Documentation 

## 2.1 Typical Steps for a CRP Project

### 2.1.1 Project level documentation

Every CRP project should contain project level documentation that includes a description of the project and site, date(s) of the survey, name(s) and organization(s) of the surveyor(s), and other useful notes. A comprehensive list of metadata needed at the project level can be found in Section 3.1 (Project Metadata) of this guide. This list of metadata is required for any close-range photogrammetry project selected for long term preservation. 

For more information about project level metadata and why it is needed, please refer to the documents, *Minimum requirements for metric use of non-metric photographic documentation* [@dayala2003] and *Recording, Documentation, and Information Management for the Conservation of Heritage Places* [@letellier2007]. 

### 2.1.2 Metric Calibration of Camera(s)

A wide variety of off-the-shelf, consumer grade digital cameras have been proven useful for close-range photogrammetry. The choice of camera(s) is usually dependent upon the accuracy requirements of the given project. Regardless of the quality or resolution of the camera and lens used, camera calibration (stand-alone or self calibration) is a required step to measure internal parameters (interior orientation) of the camera and to correct for distortions caused by the lens. 

Each calibration performed is specific to a particular camera/lens combination, and is not valid for any other camera or lens used within a project. In addition, adjusting the zoom of a lens will require a new calibration as the internal parameters (i.e. the focal length) for the camera have now changed. It is also recommended to keep a fixed focus throughout the calibration and image capture. 

A comprehensive list of metadata required for camera calibrations can be found in Section 3.2 (Camera Metadata) of this guide. This is required metadata for any camera record and/or calibration images selected for long term preservation.

### 2.1.3 Image Capture

Organization and documentation during the collection of digital images in the field is especially important. A planimetric map (sketch) illustrating the feature(s) being surveyed, the location and orientation of each image collected, and any important notes about an image (e.g. included color chart, plumb line, scale, control point etc.) is important. Basic cartographic principals should be followed, including a title, north arrow, approximate scale, legend, and appropriate notes. Documentation linking the indicated positions on the map to the digital image file name is also required. As for camera settings, most digital cameras store information about the settings and internal dimensions in what is known as the Exchangeable Image File Format (EXIF) header, and can be accessed via most image processing software (also see Section 3.3 of the [Raster Images Guide](https://doi.org/10.5284/mtgj-7130)).

There are a number of strategies for the collection of images in a photogrammetric project. Typically, the strategy is driven by the method or software used to process the images, and, more specifically, whether the processing requires a convergent or stereo set of images. In either case, the commonly accepted good practice for structures follows the 3x3 rules as detailed in the paper, *The 3x3 Rules for Simple Photogrammetric Documentation of Architecture* [@waldhausl1994].

A comprehensive list of metadata required for images taken in the field can be found in Section 3.3 (Image Metadata) of this guide. This group is required for any close-range photogrammetric images selected for long term preservation.

Other useful information about image level documentation can be found in section 4 (namely sections 4.4-4.6) of the document, *Minimum requirements for metric use of non-metric photographic documentation* [@dayala2003].

### 2.1.4 Acquisition of External Control

External control information can be added to a photogrammetric project for two reasons: 1. to provide datum information and/or 2. to provide geometric constraints on the photogrammetrically derived model.  

* __Datum definition__: If the photogrammetric model is to be situated partially or wholly within an existing reference frame or datum (geodetic, mapping or local) then sufficient external references defined in this frame must be integrated into the project.  A 3D reference frame or datum is defined by scale, position and orientation.  Typically, reference information is in the form of control points (photo-identifiable points with known coordinates in a reference frame), lengths of photo-identifiable objects, and/or angles between photo-identifiable objects.

* __Scale__: Since photogrammetric models are scale deficient, suitable scale control must be included in the project to uniquely define the size of the model in the reference frame.  This can take the form of a scale bar of known length, a measured distance on an object in two or more photos, or two control points.  In this case the accuracy of the control information determines the scale-accuracy of the photogrammetric model (although it does not affect the accuracy of the shape of the model).  

* __Position__: The position of the photogrammetric model within a reference frame is uniquely determined by a single photo-identifiable point with known 3D coordinates.  This can be determined by total station survey, GPS or other means.  The positional accuracy of the model within the reference frame is determined by the accuracy of this 3D control point within the frame.  It does not affect the scale or shape accuracy of the model.

* __Orientation__: The orientation of the photogrammetric model within a reference frame is uniquely determined by two 3D control points and a single control point for which only one coordinate (X, Y or Z) is known.  

If the minimum amount of information is provided (two 3D control points and one 1D control point) then the control will not contribute to the relative accuracy of the model except the scale (which is determined by the distance between the two 3D control points).

Apart from scale, if minimal control information is provided then it only affects the position and orientation of the photogrammetric model within the datum.  The accuracy of relative distances and angles is determined completely by the photogrammetric data.  Therefore the control information used to determine position/orientation within a reference frame could take the form of lower-accuracy observations (e.g. points derived from mapping grade GPS) as long as the placement within the frame did not require more accuracy than the control observations.  If, for example, only 2 mapping-grade GPS control points were used (say 1-meter accuracy) along with a known elevation (benchmark) were used as control, then the scale of the model would be determined by the computed distance between the points, the position would be determined based on the two control points and the orientation determined by all the control information.  A scale bar could be incorporated to determine scale to a higher accuracy.  The particular use of such varied control information should be captured in the metadata (i.e. which control element was used for each datum element).

__Geometric Constraints__: If more than minimal control is provided (e.g. three or more 3D control points) then the control information will be used to help define the shape of the photogrammetric model as well as define its datum (as above).  In this case, the surveyor must ensure that the control information is, as a rule-of-thumb, at least 3x more accurate than the photogrammetric model itself.  If it is not, then the control information will distort the photogrammetric model and potentially have deleterious effects on its relative accuracy.  For example, if the internal precision of a photogrammetric model (as derived from the bundle adjustment) is 1:1000, then the control information should be accurate to at least 1:3000.  This does not address the absolute accuracy of the control information (its accuracy within the reference frame) and the absolute position/orientation/scale of the photogrammetric model within the frame is still determined by the control information just as it is in datum definition.

Typically, control for geometric constraints is developed by total station surveys which densify (near the site) existing but sparse control information in a geodetic or mapping frame.

Metadata standards for all control should be the same.  That is, coordinates and covariance matrices describing the precision/accuracy of the coordinates.  Photographs to help locate, textual descriptions of the location, etc.

Metadata needed for any external control can be found in Section 3.4 (Reference/Datum Metadata) of this guide. This metadata is required only if external control is used within the close-range photogrammetry project. 

### 2.1.5 Image Processing

Most digital images captured in the field will require some digital processing or enhancement in order to produce the most desirable image. Processing and enhancement include any significant adjustments to the brightness, color, contrast, sharpness, or other common image properties. It is also sometimes necessary to convert a digital image from one format to another. While these processes may be necessary for a particular project to move forward, the original, unprocessed images should be submitted for archival. If the camera used is set to capture images in a proprietary RAW format, these should be converted to an archival format before submission (e.g. Nikon RAW .nef format to Adobe .dng using the Adobe DNG converter). More information on raster images can be found in Section 3.3 of the [Raster Images Guide](https://doi.org/10.5284/mtgj-7130).

One important note is to never crop (or change the height/width in any way) an image intended for photogrammetry. It is also important to document image format conversions, as these can vary depending on formats converted to or from, and on what software is used to perform the conversion. A metadata field for format conversions and can be found in Section 3.3 of this guide. 

### 2.1.6 Triangulate/Orient Block

In order to extract three dimensional points from two dimensional images, it is necessary to perform a triangulation with at least two images (a stereo pair). When more than two images are used in a triangulation, we refer to the group of images as a 'block'. To perform a triangulation, we must measure a sufficient number of tie, control, and/or check points throughout the block. Constraints may also be placed on certain sets of points to enforce angular, linear, and/or planar properties.

Once a triangulation is successful, image exterior orientation parameters (along with estimate for accuracy) should be available to the user. These are important pieces of information for downstream deliverables and should be documented. Information on metadata needed at the model level can be found in Section 3.5 (Model Metadata) of this guide. This group will be required for any end product selected for long term preservation.

### 2.1.7 Deliverable Creation

Typical deliverables created as the end result of a CRP project could include stereo pairs, 2D vector graphics (2D CAD models), dense point clouds, CAD-like or facetized models of an object or surface, or raster graphics such as rectified or fully orthorectified images. Each deliverable that is selected for preservation should include all of the above mentioned metadata groups, as well as metadata for the additional processing performed to create the file. 

Metadata needed for 2D vector graphics (2D CAD models), dense point clouds, and facetized models can be found in Section 3.4 of the [Laser Scanning guide](https://doi.org/10.5284/rt5g-dm24) and Section 4.6 of the [CAD guide](https://doi.org/10.5284/k5hd-hj61). 

```{figure} ../images/CRPworkflow-large.png
:alt: Figure 1

__Figure 1:__ The close-range digital photogrammetry workflow.
```