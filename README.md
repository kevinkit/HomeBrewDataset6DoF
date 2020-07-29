# HomeBrewDataset6DoF
This repository is for using a 6DoF dataset which was labeled automatically using camera intrinsics.

# Dataset

This dataset has 9 different objects, in total there are 126.520 images - however only 59.376 are labeled due to the low quality of the remaining ones. 
These images were labeled automatically, this is why some of the cuboids may be a little bit off. The unlabeled images are in the Image archives, so there will be more images than ground truth files. 

The camera parameters can be downloaded from: [camera Parameters](https://drive.google.com/drive/folders/1w_kA6w2Uqxs8oMWpOsYr3mgfr0BgU8S3?usp=sharing). 
The measurements of the objects can be downloaded from: [measurements](https://drive.google.com/drive/folders/1j3WGH4kHVu-2m5xHDwGgdfNB3FDaXK69?usp=sharing).
The ground truths can be downloaded from: [ground Truth](https://drive.google.com/drive/folders/19ct2qqfoeUZS_BqgBDQCbJjOiIRfcT2m?usp=sharing).


The images can be downloaded from the following table:
| Class Name | Images | 
|------------|--------|
|BeerMug     |[BeerMug](https://drive.google.com/file/d/1j1jPM_pRs2KLma58jY3xd7NVL3A3tYSB/view?usp=sharing)     |   
|can            |[can](https://drive.google.com/file/d/1Zpf4VvvEqL7VDXnL2pBkiM5VHgYHJyxl/view?usp=sharing)        |            
|CircuitBoard       | [CircuitBoard](https://drive.google.com/file/d/1kwmnZ2Zyt2A2T7CHDxsdy-1gfOJ3RflN/view?usp=sharing) |                     
|clock              |[clock](https://drive.google.com/file/d/1aRlDbgjRFfjzS8NK0L0mAcmfJPk7u7j7/view?usp=sharing)|                        
|Coal               |[Coal](https://drive.google.com/file/d/1gaqLUXIH3-O_Mw35WEEAUpzWocFGjwA6/view?usp=sharing)|                          
|CoffeCup           |[CoffeCup](https://drive.google.com/file/d/1ig_V9wu0UPgYLpltqDgHc_1M6CVwIY3d/view?usp=sharing)|                          
|decorativeBulbOff  |[decorativeBulbOff](https://drive.google.com/file/d/1SMJQuBjJ7VVS5E77dkPkD0ZUut1KnoG0/view?usp=sharing) |                          
|decorativeBulbOn   |[decorativeBulbOn](https://drive.google.com/file/d/1XRCeJJHYS7Y5aW7uoMJ_U7KC8ELWgkkd/view?usp=sharing)|                          
|scotchTape         |[scotchTape](https://drive.google.com/file/d/1JZmUl3TqjIBNh6Oi7rzpyJ7o6emFU0mU/view?usp=sharing)|            

# Labels

The label files are .json files. The name of the files are the same as the images. The following keys are available in the json file:


| key name | Usage |
|----------|-------|
| frame_name | This is the name of the corresponding image | 
| objectPoints3D | These are the 3D coordinates of the object in xyz order of the object|
| objectPoints2D | These are the transformed 2D coordinates on the image plane of the object|
| quaternion | This is the quaternion describing the rotation of the object. The first element is the imaginary part |
| translation | This is the translation vector of the object |
| camera_matrix | This is the intrinsic camera matrix, it will be the same over all images|
| discoef | These are the coefficients of the camera |
| paper3D | The objects are placed on a white paper, these are the 3D coordianates of the paper | 
| paper2D | The objects are place on a white paper, these are the projected 2D coordinates of the paper |

# Citation

If you find this dataset useful or use it in your research please cite:

```
@misc{khoefle2020,
  author = {Kevin Hoefle},
  title = {HomeBrewDataset6DoF},
  year = {2020},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/kevinkit/HomeBrewDataset6DoF}},
}
```

# Support

If you want to support the hosting of this dataset and the development of further helping functions, you can [donate](https://www.paypal.com/paypalme/happydonations)


