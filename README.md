# PyRicianNormalization
MRI image normalization scheme based on Rice distribution 

# Introduction
RicianNormalization is a tool that reads T2W images (as DICOM or Nifti, MetaIO, etc...) and potentially other magnitude MR images, fits a Rice distribution to the pixel intensities and normalizes the pixels based on the standard score using the fit Rice mean and standard deviation.

PyRicianNormalization is a Python port of RicianNormalization

https://github.com/nslay/RicianNormalization

The method is loosely based on this work:
Lemaître, Guillaume, et al. "Normalization of t2w-mri prostate images 
using rician a priori." Medical Imaging 2016: Computer-Aided Diagnosis. 
Vol. 9785. International Society for Optics and Photonics, 2016.

Though the implementation is vastly different employing a maximum log
likelihood scheme to fit the Rice distribution.

# Installing
TODO

# Usage
TODO

# Caveats
Saving floating point voxel output to DICOM series does not seem to work correctly. Limitation of SimpleITK?
