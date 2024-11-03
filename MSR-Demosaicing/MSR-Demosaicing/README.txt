Microsoft Demosaicing Dataset
Data set and results

Description 
==========================================
The Microsoft Research Cambridge demosaicing data set consists of set of raw images, and their downscaled versions which can be used for learning and evaluating demosaicing (and possibly other tasks like denoising), both in linear-space and color-space.

Other details could be found at the dataset webpage: 
http://research.microsoft.com/en-us/um/cambridge/projects/msrdemosaic/

By installing, copying, or otherwise using this software, you agree to be bound by the terms of its license. Read the "License.txt" for the details.

This package the following items:

1) raw images 
==========================================
See the contents of the folder 'Raw_Images'. 
The raw images are taken by two different cameras: 
- Panasonic Lumix DMC-LX3 : 'Raw_Images\panasonic' folder 
- Canon EOS 550D : 'Raw_Images\canon' folder 
The major portion of the images are taken by Panasonic camera which can be used for training of a machine learning model for demosaicing(or denoising). 

The raw images are preprocessed with Dave Coffin's dcraw: 
- <http://www.cybercom.net/~dcoffin/dcraw/>

The outputs of the dcraw are also included in the same folder: 
- 'Images\raw_tiff_panasonic-4DwT'
- 'Images\raw_tiff_canon-4DwT'

Also, the parameters of each image are extracted, which can be used for down-scaling, training, and evaluation. 
- 'Raw_Images\panasonic-params'
- 'Raw_Images\canon-params' 


2) Evaluation script and camera pipeline
==========================================
The folder 'Codes\EvaluationAndCameraPipeline' contains the evaluation scripts and the functionalities for simulating the camera pipeline for LINEAR-space images. See the folder for more information. 


3) Downscaling raw images 
==========================================
We have included samples scripts for downscaling raw-images, and creating smaller-sized ground-truth images. For more details refer to the folder: 'Codes\Downscaling'


People 
===============
Daniel Khashabi, UIUC
Sebastian Nowozin, MSCR
Jeremy Jancsary, Nuance 
Andrew Fitzgibbon, MSRC

Reference 
===============
Please cite the following paper if you are using this database. 

@article{rtfDemosaicing2013,
  title={Joint Demosaicing and Denoising via Learned Non-parametric Random Fields},
  author={Khashabi, Daniel and Nowozin, Sebastian and Jancsary, Jeremy and Fitzgibbon, Andrew},
  note={Image Processing, IEEE Transactions on},
  year={2014}
}
