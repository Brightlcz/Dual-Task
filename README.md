# Reference-based Dual-Task Framework for Motion Deblurring
by Cunzhe Liu, Zhen Hua, Jinjiang Li.

Pytorch Implementation of "Reference-based Dual-Task Framework for Motion Deblurring"
![Overview of Framework](./docs/dusk.png)

## Dependency
This code is based on PyTorch 1.1 and CUDA 10.0. It has been tested on Ubuntu 18.04 LTS, where the machine is equipped with NVIDIA Titan RTX GPUs.
We use Anaconda to set up the environment. Users can set up a new environment simply by:

```
conda create -n 1.11 python=3.7
conda activate 1.11
conda install pytorch==1.1.0 torchvision==0.3.0 cudatoolkit=10.0 -c pytorch
```

Then, users need to install the deformable convolution module in the `1.11` environment by:

```bash
cd dcn
python setup.py develop
```

If you got an error when installing deformable convolution module, please delete the `build` folder first and then run:

```bash
cd dcn
rm -rf build
python setup.py build develop
```

## Results
The deblurring results of Dual-Task on GrPro test set:
The deblurring results of Dual-Task on HIDE test set:
