# NCTU_hw4
Implementation of super-resolution using [DRRN](https://openaccess.thecvf.com/content_cvpr_2017/papers/Tai_Image_Super-Resolution_via_CVPR_2017_paper.pdf).

## Environment:
-Python 3.6  
-PyTorch 1.5  


## Usage:

### Preparing training dataset  
  - download the [data](https://drive.google.com/drive/u/0/folders/1H-sIY7zj42Fex1ZjxxSC3PV1pK4Mij6x)
  - the training data is generated with Matlab Bicubic Interpolation, please refer [Code for Data Generation](/data/generate_trainingset_x234.m) for creating training files.  
  
### Training:  
  -run the following command to train:  
   python train.py --dataset (the dataset you want to train) --outdirname (the output directory)
   
### Generate pictures:
  -run the following command to generate sr-pictures:  
   python sr.py --model model_7000.npz --image x.png, x is the number of the picture


