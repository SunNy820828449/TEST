TensorRT backend for Espnet ASR Transformer.
====

dependency
----
TensorRT plugin is required.

##building

    install TensorRT-7.0

    git clone -b release/7.0 --recursive https://git.sysop.bigo.sg/sunli/TensorRT.git

    cd TensorRT && mkdir build && cd build

    cmake .. -DTRT_LIB_DIR=$TRT_RELEASE/lib -DTRT_BIN_DIR=`pwd`/out

    make -j


c++
----
c++ code for tensorrt execution

##using python api

    python3 espnet2trt.py #using --help to see options

      note: mk.sh is script for building c++ code

python
----
python code for tensorrt execution

##using

    python3 espnet_transformer_trt.py is not ready

    python3 espnet_lm_trt.py #using --help to see options

