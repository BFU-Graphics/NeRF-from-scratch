# Neural Radiance Fields, From Theory to Implementation.

## Setup

Prerequisites:

- Python3.10
- CUDA 11.7

First, download  [Synthetic NeRF dataset](https://dl.fbaipublicfiles.com/nsvf/dataset/Synthetic_NeRF.zip) and unzip it under the root dir.

Then, setup pip venv environment.

1. `pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117`
2. `python -m pip install -U pip`
3. `pip install -i https://pypi.taichi.graphics/simple/ taichi-nightly`
4. `pip install -r requirements.txt`

run train.py with parameters:

`python train.py --root_dir ./Synthetic_NeRF/Lego --exp_name Lego --perf --num_epochs 20 --batch_size 512 --lr 1e-2 --no_save_test --gui`

## Volume Rendering

- https://www.scratchapixel.com/lessons/3d-basic-rendering/volume-rendering-for-developers/intro-volume-rendering.html

## NeRF

- https://github.com/awesome-NeRF/awesome-NeRF