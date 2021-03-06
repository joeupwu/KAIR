## Training and testing codes for DnCNN, FFDNet, SRMD, DPSR, MSRResNet, ESRGAN, IMDN


**News**: [USRNet (CVPR 2020)](https://github.com/cszn/USRNet) will be added.
_______

Training
----------
- [main_train_dncnn.py](main_train_dncnn.py) --------------- [https://github.com/cszn/DnCNN](https://github.com/cszn/DnCNN)
- [main_train_fdncnn.py](main_train_fdncnn.py) -------------- [https://github.com/cszn/DnCNN](https://github.com/cszn/DnCNN)
- [main_train_ffdnet.py](main_train_ffdnet.py) --------------- [https://github.com/cszn/FFDNet](https://github.com/cszn/FFDNet)
- [main_train_srmd.py](main_train_srmd.py) ---------------- [https://github.com/cszn/SRMD](https://github.com/cszn/SRMD)
- [main_train_dpsr.py](main_train_dpsr.py) ----------------- [https://github.com/cszn/DPSR](https://github.com/cszn/DPSR)
- [main_train_msrresnet_psnr.py](main_train_msrresnet_psnr.py) ----- [https://github.com/xinntao/BasicSR](https://github.com/xinntao/BasicSR)
- [main_train_msrresnet_gan.py](main_train_msrresnet_gan.py) ------ [https://github.com/xinntao/ESRGAN](https://github.com/xinntao/ESRGAN)
- [main_train_rrdb_psnr.py](main_train_rrdb_psnr.py) ----------- [https://github.com/xinntao/ESRGAN](https://github.com/xinntao/ESRGAN)
- [main_train_imdn.py](main_train_imdn.py) ---------------- [https://github.com/Zheng222/IMDN](https://github.com/Zheng222/IMDN)

Network architectures
----------
* [USRNet](https://github.com/cszn/USRNet)

#TODO

* DnCNN

  <img src="https://github.com/cszn/DnCNN/blob/master/figs/dncnn.png" width="600px"/> 

* FFDNet

  <img src="https://github.com/cszn/FFDNet/blob/master/figs/ffdnet.png" width="600px"/> 

* SRMD

  <img src="https://github.com/cszn/SRMD/blob/master/figs/architecture.png" width="605px"/> 

* SRResNet, SRGAN, RRDB, ESRGAN

  <img src="https://github.com/xinntao/ESRGAN/blob/master/figures/architecture.jpg" width="595px"/> 
  
* IMDN

  <img src="figs/imdn.png" width="460px"/>  ----- <img src="figs/imdn_block.png" width="100px"/> 



Testing
----------
- [main_test_dncnn.py](main_test_dncnn.py) ---------------> ```model_zoo: dncnn_15.pth, dncnn_25.pth, dncnn_50.pth, dncnn_gray_blind.pth, dncnn_color_blind.pth, dncnn3.pth```
- [main_test_fdncnn.py](main_test_fdncnn.py) --------------> ```model_zoo: fdncnn_gray.pth, fdncnn_color.pth, fdncnn_gray_clip.pth, fdncnn_color_clip.pth```
- [main_test_ffdnet.py](main_test_ffdnet.py) ---------------> ```model_zoo: ffdnet_gray.pth, ffdnet_color.pth, ffdnet_gray_clip.pth, ffdnet_color_clip.pth```
- [main_test_srmd.py](main_test_srmd.py) ----------------> ```model_zoo: srmdnf_x2.pth, srmdnf_x3.pth, srmdnf_x4.pth, srmd_x2.pth, srmd_x3.pth, srmd_x4.pth``` ```The above models are converted from MatConvNet. ```
- [main_test_dpsr.py](main_test_dpsr.py) -----------------> ```model_zoo: dpsr_x2.pth, dpsr_x3.pth, dpsr_x4.pth, dpsr_x4_gan.pth```
- [main_test_msrresnet.py](main_test_msrresnet.py) -----------> ```model_zoo: msrresnet_x4_psnr.pth, msrresnet_x4_gan.pth```
- [main_test_rrdb.py](main_test_rrdb.py) -----------------> ```model_zoo: rrdb_x4_psnr.pth, rrdb_x4_esrgan.pth```
- [main_test_imdn.py](main_test_imdn.py) ----------------> ```model_zoo: imdn_x4.pth```

[model_zoo](model_zoo)
--------
- download link [https://drive.google.com/drive/folders/13kfr3qny7S2xwG9h7v95F5mkWs0OmU0D](https://drive.google.com/drive/folders/13kfr3qny7S2xwG9h7v95F5mkWs0OmU0D)

[trainsets](trainsets)
----------
- [https://github.com/xinntao/BasicSR/wiki/Prepare-datasets-in-LMDB-format](https://github.com/xinntao/BasicSR/wiki/Prepare-datasets-in-LMDB-format)
- [train400](https://github.com/cszn/DnCNN/tree/master/TrainingCodes/DnCNN_TrainingCodes_v1.0/data)
- [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/)
- [Flickr2K](https://cv.snu.ac.kr/research/EDSR/Flickr2K.tar)
- optional: use [split_imageset(original_dataroot, taget_dataroot, n_channels=3, p_size=512, p_overlap=96, p_max=800)](https://github.com/cszn/KAIR/blob/3ee0bf3e07b90ec0b7302d97ee2adb780617e637/utils/utils_image.py#L123) to get ```trainsets/trainH``` with small images for fast data loading

[testsets](testsets)
-----------
- [https://github.com/xinntao/BasicSR/wiki/Prepare-datasets-in-LMDB-format](https://github.com/xinntao/BasicSR/wiki/Prepare-datasets-in-LMDB-format)
- [set12](https://github.com/cszn/FFDNet/tree/master/testsets)
- [bsd68](https://github.com/cszn/FFDNet/tree/master/testsets)
- [cbsd68](https://github.com/cszn/FFDNet/tree/master/testsets)
- [kodak24](https://github.com/cszn/FFDNet/tree/master/testsets)
- [srbsd68](https://github.com/cszn/DPSR/tree/master/testsets/BSD68/GT)
- set5
- set14
- cbsd100
- urban100
- manga109


References
----------
```
@inproceedings{zhang2020deep, % USRNet
  title={Deep unfolding network for image super-resolution},
  author={Zhang, Kai and Van Gool, Luc and Timofte, Radu},
  booktitle={IEEE Conference on Computer Vision and Pattern Recognition},
  pages={0--0},
  year={2020}
}
@article{zhang2017beyond, % DnCNN
  title={Beyond a gaussian denoiser: Residual learning of deep cnn for image denoising},
  author={Zhang, Kai and Zuo, Wangmeng and Chen, Yunjin and Meng, Deyu and Zhang, Lei},
  journal={IEEE Transactions on Image Processing},
  volume={26},
  number={7},
  pages={3142--3155},
  year={2017}
}
@article{zhang2018ffdnet, % FFDNet, FDnCNN
  title={FFDNet: Toward a fast and flexible solution for CNN-based image denoising},
  author={Zhang, Kai and Zuo, Wangmeng and Zhang, Lei},
  journal={IEEE Transactions on Image Processing},
  volume={27},
  number={9},
  pages={4608--4622},
  year={2018}
}
@inproceedings{zhang2018learning, % SRMD
  title={Learning a single convolutional super-resolution network for multiple degradations},
  author={Zhang, Kai and Zuo, Wangmeng and Zhang, Lei},
  booktitle={IEEE Conference on Computer Vision and Pattern Recognition},
  pages={3262--3271},
  year={2018}
}
@inproceedings{zhang2019deep, % DPSR
  title={Deep Plug-and-Play Super-Resolution for Arbitrary Blur Kernels},
  author={Zhang, Kai and Zuo, Wangmeng and Zhang, Lei},
  booktitle={IEEE Conference on Computer Vision and Pattern Recognition},
  pages={1671--1681},
  year={2019}
}
@InProceedings{wang2018esrgan, % ESRGAN, MSRResNet
    author = {Wang, Xintao and Yu, Ke and Wu, Shixiang and Gu, Jinjin and Liu, Yihao and Dong, Chao and Qiao, Yu and Loy, Chen Change},
    title = {ESRGAN: Enhanced super-resolution generative adversarial networks},
    booktitle = {The European Conference on Computer Vision Workshops (ECCVW)},
    month = {September},
    year = {2018}
}
@inproceedings{hui2019lightweight, % IMDN
  title={Lightweight Image Super-Resolution with Information Multi-distillation Network},
  author={Hui, Zheng and Gao, Xinbo and Yang, Yunchu and Wang, Xiumei},
  booktitle={Proceedings of the 27th ACM International Conference on Multimedia (ACM MM)},
  pages={2024--2032},
  year={2019}
}
@inproceedings{zhang2019aim, % IMDN
  title={AIM 2019 Challenge on Constrained Super-Resolution: Methods and Results},
  author={Kai Zhang and Shuhang Gu and Radu Timofte and others},
  booktitle={IEEE International Conference on Computer Vision Workshops},
  year={2019}
}
```
