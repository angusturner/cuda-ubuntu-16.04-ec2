# Steps to install Pytorch on Amazon GPU Instance with Ubuntu 16.04 


## CUDA Installation
1. Run ```sudo apt-get update && sudo apt-get upgrade```
2. Run ```./setup_cuda.sh``` and follow the prompts:
    - Say no to 32-bit driver support and DKMS
3. Refresh bash ```source ~/.bashrc```

## Python Installation
1. Run ```./setup_python.sh```
	- NOTE: you may have to run a 2nd time after doing ```~/.bashrc```
2. Run ```source activate cuda``` to enter conda environment
3. (optional) Run ```./pip_deps.sh```
4. Run ```./setup_pytorch.sh```


## NOTES
You can check CUDA installation by typing ```nvidia-smi```. If the installation fails, you should run ```./purge_cuda.sh``` and start again. 
