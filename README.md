# STCNet
[**Paper**]([https://link.springer.com/article/10.1007/s13534-023-00309-4](https://www.sciencedirect.com/science/article/abs/pii/S001048252401610X))<br>
Yang, Jaemo, Doheun Cha, Dong-Gyu Lee, and Sangtae Ahn. "STCNet: Spatio-Temporal Cross Network with subject-aware contrastive learning for hand gesture recognition in surface EMG." Computers in Biology and Medicine 185 (2025): 109525.


### data process

first, download dataset (NinaPro DB1, DB2, DB4)
https://ninapro.hevs.ch/

second, you have to run denosing.m file!

finally
```
python emg_process.py --dataset nina1 --path 'your dataset folder path'
```

### how to run train file

```
python train_sac.py --dataset nina1 --gamma 0.3 --cosine
python train_ce.py --dataset nina1 --cosine --encoder "put your result pth file from train_multi.py"
```


### how to test

```
python test.py --dataset nina2 --model_path 'put result pth file'
```
