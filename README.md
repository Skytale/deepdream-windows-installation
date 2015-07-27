# deepdream

This is for experimenting with the Google [DeepDream](https://github.com/google/deepdream/blob/master/dream.ipynb) network.

I managed to run the deepdream network with CUDA acceleration on Windows, using [this build for the Python wrappers](
https://github.com/drakh/caffe-win-python-anaconda/)

I used Anaconda 2.7, together with CUDA 7 on Windows 8.1. I needed to install protobuf using:
"conda install -c https://conda.binstar.org/dhirschfeld protobuf"