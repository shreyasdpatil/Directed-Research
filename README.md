# Generating conductivity maps from T1-MR images of human brain using 3D autoencoder like architectures

Usage:

To run the ipython notebook put the notebook and Experimental2 data in the same folder.
The recommended way of running the notebook is in the google colab.

Requirements to generate data:

1) Install BrainSuite software
2) Install SimNIBS software

Generate Data:

1) Generate bias-field-corrected images

```
example
bfc -i input_mri.nii.gz -o output_mri.bfc.nii.gz
```

2) Genrate coregistered diffusion MRI

```
bdp.sh <BFC File> [Optional Flags] --nii <4D DWI NIfTI> -g <Gradient File> -b <B-Value File>
```

For more information read 4.4 in DR_Report.pdf

Dataset can be accessed at:

https://drive.google.com/drive/folders/1tyRSqA0LHC6VK483JqTTITqfo0RALUTF?usp=sharing
