FROM nvidia/cuda:11.8.0-devel-ubuntu22.04

RUN apt-get update
RUN apt-get install -y \
    build-essential \
    python3-dev \
    python3-pip \
    git

RUN pip3 install torch==2.0.0 --extra-index-url https://download.pytorch.org/whl/cu118
RUN pip3 install torch-geometric==0.4.0 -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
RUN pip3 install numpy==1.26.4 h5py==3.11.0 tensorboard==2.16.2 scipy==1.11.0 scikit-learn==1.4.2 mkl==2024.1.0 sparse-dot-mkl==0.9.3

