apt update && apt upgrade -y && apt install pve-headers-$(uname -r) build-essential software-properties-common make nvtop htop -y
./NVIDIA-Linux-x86_64-570.169.run --dkms

OPTIONAL
@reboot nvidia-smi -pm 1 && nvidia-smi -pl 250
