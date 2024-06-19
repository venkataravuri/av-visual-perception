# Autnomous Vehicle
Credits: https://medium.com/@shahrullo/visual-perception-for-self-driving-cars-bb500f8c6adc

Visual Perception for Self-Driving Cars!

## Installation

wget https://repo.anaconda.com/archive/Anaconda3-2024.02-1-Linux-x86_64.sh

bash Anaconda3-2024.02-1-Linux-x86_64.sh

eval "$(/home/ubuntu/yes/bin/conda shell.bash hook)" 

Create new conda environment
conda create -n .venv python=3.9 jupyter

conda activate .venv


## Create AWS EC2 launch template with NVIDIA Drivers, CUDA and Conda

sudo lshw -c video

sudo apt-get install -y ubuntu-drivers-common
sudo ubuntu-drivers install

sudo reboot

nvidia-smi

sudo apt-get update -y
sudo apt-get install build-essential libgl1 unzip -y
sudo apt-get install linux-headers-$(uname -r)

# Verify machine has CUDA-Capable GPU
lspci | grep -i nvidia
# Verify You Have a Supported Version of Linux
uname -m && cat /etc/*release
# Verify the System Has gcc Installed
gcc --version

sudo apt-get install nvidia-cuda-toolkit -y

nvcc --version