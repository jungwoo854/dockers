FROM soonminh/baseenv:mat-py-cuda7.0-cudnn4
 
 MAINTAINER Soonmin Hwang <smhwang@rcv.kaist.ac.kr>
 
 # 0. INSTALL Caffe dependencies
 RUN apt-get update 
 RUN apt-get install -y \ 
 	 libprotobuf-dev libleveldb-dev libsnappy-dev libopencv-dev libhdf5-serial-dev protobuf-compiler 
 RUN apt-get install -y --no-install-recommends libboost-all-dev 
 RUN apt-get install -y libgflags-dev libgoogle-glog-dev liblmdb-dev 
 RUN apt-get install -y libatlas-base-dev libopenblas-dev 
 
 # 1. Clone PSPNet repository
 RUN git clone https://github.com/hszhao/PSPNet.git /home/rcvlab/PSPNet && \ 
 	 chown -R rcvlab:rcvlab /home/rcvlab/PSPNet
 
 RUN ["/bin/bash"]
