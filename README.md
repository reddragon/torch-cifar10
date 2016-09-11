# Torch CIFAR-10 Demo

Mostly blatantly copied from @soumith's [Deep Learning Intro with Torch](https://github.com/soumith/cvpr2015/blob/master/Deep%20Learning%20with%20Torch.ipynb).

## Dependencies
* `nn` for Neural Nets, obviously.
* `clnn`, `cltorch` if using OpenCL
* `cunn`, `cutorch` if using CUDA


## Demo
* If you want to run the demo on your CPU, try `th cifar10.lua`.
* For GPUs, figure out which & how many GPUs you have via `lspci | grep NVIDIA` or `lspci | grep AMD`.
* `th cifar10.lua -gpu 0 -backend cunn` - Will run the demo on your NVIDIA GPU number 1 (0-indexed).
* `th cifar10.lua -gpu 0 -backend clnn` - Will run the demo on your AMD GPU number 1 (0-indexed).

