FROM nvidia/cuda:11.8.0-devel-ubuntu22.04

RUN apt-get update
RUN apt-get install -y \
    build-essential \
    python3-dev \
    python3-pip \
    intel-mkl-full \
    git

RUN pip3 install torch --extra-index-url https://download.pytorch.org/whl/cu118
RUN pip3 install torch-cluster torch-scatter torch-sparse torch-geometric -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
RUN pip3 install numpy h5py tensorboard scipy==1.11.0 scikit-learn sparse-dot-mkl

