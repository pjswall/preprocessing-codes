# Preprocessing for Morphing data

Preprocessing codes for Morphing Project 

<img src="https://github.com/prateekj7777/Morphing/blob/main/arch..jpg" width="500px" height="300px" alt="architecture.jpg" align=center />
</div>
</br>

# Requirements
Please install following packages 
- numpy= 1.11.0
- torch=1.9.-
- torchvision=0.10.0
- deepface=0.0.74
- Pillow==3.1.2
- psutil==3.4.2
- matplotlib

# How to RUN
1. Download the data files for the required model. Extract and place it in the data folder.
2. Create a new virtual environment

using conda:
```
>>> conda create -n <env-name>
```
using pip
```
>>> python -m pip install --user virtualenv
```
4. Install the required packages using the requirements.txt file with the following command
```
>>> pip install -r requirements.txt
```


# Dataset

We have used two face morph datasets.

### AMSL Dataset

This dataset contains morph images from 102 subjects captured with neutral as well as smiling expressions. Thare are 2175 morphed images corresponding to 92 subjects created using a landmark-based approach. 

### E-MorGAN Dataset


This dataset created using GAN's and all the morphed images are generated with the GAN architecture called MorGAN. Dataset is having at 1000 images which are splittes as train and test sets of 500 images in each set.

Dataset specification
---------------------


| Dataset 	| split 	| Morphed/Non-morphed 	| no. of species | No. of images
|---	|---	|---	|---  |---
| AMSL | Train | Morphed | 73 | 946
| AMSL | Test | Morphed | 16 | 56
| AMSL | Test | Non-morphed | 29 | 57
| E-MorGAN | Train | Morphed | 251 | 499
| E-MorGAN | Test | Morphed | 90 | 100
| E-MorGAN | Test | Non-morphed | 50 | 100

Here, the required details about each dataset presented in the below table.

# References

This repo will work for [ Facial-Demorphing : Extracting Component Faces from a Single Morph](https://arxiv.org/abs/2209.02933v1#:~:text=The%20task%20of%20deducing%20the%20individual%20face%20images,of%20the%20accomplice%20-%20i.e.%2C%20the%20other%20identity.) mentioned in the reference paper.

