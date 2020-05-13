# SAC-Net: Spatial Attenuation Context for Salient Object Detection


by Xiaowei Hu, Chi-Wing Fu, Lei Zhu, Tianyu Wang, and Pheng-Ann Heng.

This implementation is written by Xiaowei Hu at the Chinese University of Hong Kong.

***

## Citation

@article{hu2020sac,                  
&nbsp;&nbsp;&nbsp;&nbsp;  author = {Hu, Xiaowei and Fu, Chi-Wing and Zhu, Lei and Wang, Tianyu and Heng, Pheng-Ann},      
&nbsp;&nbsp;&nbsp;&nbsp;  title = {SAC-Net: Spatial Attenuation Context for Salient Object Detection},      
&nbsp;&nbsp;&nbsp;&nbsp;  journal = {IEEE Transactions on Circuits and Systems for Video Technology},        
&nbsp;&nbsp;&nbsp;&nbsp;  year = {2020},                     
&nbsp;&nbsp;&nbsp;&nbsp;  note = {to appear},                    
}
   
## Saliency Maps

Please find the predicted saliency maps on the ECSSD, PASCAL-S, SOD, HKU-IS, DUT-OMRON, and DUTS-test at [Google Drive](https://drive.google.com/open?id=1Z2WV39lxeyDBXlpNFhoxYgOmwWsoQutX).


## Installation

1. Please download and compile our [CF-Caffe](https://github.com/xw-hu/CF-Caffe).

2. Put the `examples/SAC-Net/` into `CF-Caffe/examples/`.

  
## Train

Download the ResNet-101 or ResNet-50 model trained on the ImageNet and put this model in `CF-Caffe/models/`.

1. Enter the `./examples/SAC-Net/SAC-Net-res101/` or  `./examples/SAC-Net/SAC-Net-res50/`.
   Modify the image path in `train_val.prototxt`.

2. Run   
   ```shell
   sh train.sh
   ```


## Test   
1. Please download our pretrained model at [Google Drive](https://drive.google.com/open?id=1FLehQ4iX0qdm6shwN4Cp0L2EzVPAXNZW).   
   Put this model in `./examples/SAC-Net/SAC-Net-res101/snapshot/`.

2. Enter the `./examples/` and run `test_saliency.m` in Matlab. 

