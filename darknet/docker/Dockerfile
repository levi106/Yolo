FROM nvidia/cuda:8.0-cudnn6-devel-ubuntu16.04

MAINTAINER Hiroyuki Hasebe crystalline407@gmail.com

RUN \
    apt-get update && apt-get install -y \
    autoconf \
    automake \
    libtool \
    build-essential \
    git

RUN \
    apt-get install -y \
    wget

RUN \
    git clone https://github.com/pjreddie/darknet

WORKDIR darknet/

RUN \
    make

RUN \
    wget http://pjreddie.com/media/files/yolov2.weights 

CMD ["bash"]

