# CudaOnHybrydNOtebooks
Some files and configurations to achieve the use of CUDA on Hybrid (Intel + Nvidia) Notebooks.

Notebook Model: Lenovo Y50-70
$ sudo apt-add-repository ppa:graphics-drivers/ppa
$ sudo apt-add-repository ppa:bumblebee/testing
# apt install nvidia-384
Install CUDA 9.0 from Nvidia .run file, dont install driver
Put following lines at end of /etc/bash.bashrc :
export CUDA_PATH=/usr/local/cuda-9.0
export PATH=/usr/local/cuda-9.0/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/cuda-9.0/lib64:$LD_LIBRARY_PATH
export LD_LIBRARY_PATH=/usr/local/cuda-9.0/include:$LD_LIBRARY_PATH
export PATH=/usr/lib/nvidia-384/bin:$PATH

at file .bashrc add: 
export CUDADIR=/usr/loca/cuda

correct bumblebee configurations and modeprobe configurations (some are automatically generated), check this initial repo: 
