# Visualizing DNA folding and RNA in embryos at single-cell resolution
 
Leslie J. Mateo[1], Sedona E. Murphy[1,2], Antonina Hafner[1], Isaac S. Cinquini[1,3], Carly A. Walker[1], Alistair N. Boettiger[1,4]

1. Department of Developmental Biology, Stanford University
2. Department of Genetics, Stanford University
3. Department of Computer Science, Stanford University
4. address correspondence to: boettiger@stanford.edu


## ORCA Data
This repository contains data associated with our manuscript, "Visualizing DNA folding and RNA in embryos at single-cell resolution", which is currently under review.  The corresponding experiments, results and conclusions are described in detail in the main text and associated methods of the paper. These data come from experiments using Optical Reconstruction of Chromatin Architecture (ORCA), an approach which is described in detail in the manuscript.

Please note, we are working to develop an easier format and interface for sharing these data, which will facilitate integration of the DNA barcode 3D positions with the cell-segmentation, embryo-position, mRNA localization, and nascent RNA quantification described in the manuscript.  

The data are provided here as a single csv files per experiment. The resolution of the experiment and the genotype of the embryos analyzed are indicated in the file name.  

## Data structure
* This repository contains the nanoscale *x*, *y*, *z* coordinates (in nanometers) of the all barcodes localized during ORCA in our unpublished manuscript. These positions are measured relative to the position on the camera-frame, which is recorded in columns *locusX* and *locusY*. The field of view is recorded in column *fov*. The index of the barcode is in column *read*
* Fiducial correction information is recorded in units of pixels in the columns *xshift*, *yshift* and *zshift* and the the centroid of the fiducial image is recorded in columns *fid\_x*, *fid\_y* and *fid\_z*.    
* Additional columns contain information on the quality of the Gaussian fitting of the pointspread function detected on the labeled barcode. These include the intensity peak of the spot *h*, the gaussian widths (sigma) are recorded as *wx*, *wy*, *wz* in nanometers and the upper and lower 95% uncertainty bounds in position (prior to drift correction) are recorded as in nanometers as *xL*, *xU* for the lower and upper limits respectively. 

## Additional Manuscript Data
* The raw image files require 12.33 Tb of data storage and are available upon reasonable request. 
