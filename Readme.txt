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