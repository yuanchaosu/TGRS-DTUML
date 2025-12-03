@ARTICLE{11271725,
  author={Su, Yuanchao and Li, Sheng and Zhou, Yicong and Gao, Lianru and Jiang, Mengying and Sun, Xu and Li, Haiwei and Hou, Enke},
  journal={IEEE Transactions on Geoscience and Remote Sensing}, 
  title={Dilated Transformation-Guided Unsupervised Multimodal Learning for Hyperspectral and Multispectral Image Fusion}, 
  year={2025},
  volume={},
  number={},
  pages={1-1},
  keywords={Convolution;Hyperspectral imaging;Superresolution;Spatial resolution;Training;Optical imaging;Image fusion;Data models;Sparse matrices;Optical sensors;Hyperspectral and Multispectral Image Fusion;Hyperspectral Image Super-resolution;Dilated Convolution;Multimodal Fusion;Multimodal Learning},
  doi={10.1109/TGRS.2025.3636047}}

## Training

1. Start visdom first in one terminal
```
visdom --port=8097
```

2. Bring up the page localhost:8097 in your browser

3. Run shell file in another terminal
```
sh bash.sh
```
--name=TG
--model_name=fusion
--gpu_ids=0
--num_theta=100
--sigma=0.5
--niter=2000
--niter_decay=8000
--lr=3e-3
--lr_policy=lambda
--lr_decay_gamma=0.8
--lr_decay_iters=1000
--display_port=8097
--lambda_A=10
--lambda_B=10
--lambda_C=10
--lambda_D=0.01
--lambda_E=0.01
--lambda_F=100
--data_name=TG
--scale_factor=8
--print_freq=20
--batchsize=1

--which_epoch=9000

