Experiments with the Google [DeepDream](https://github.com/google/deepdream/blob/master/dream.ipynb) network.

## Script enhancements

In 'Dream Multiple.ipynb' I have made a few modifications to the original Google script
- It is possible to specify multiple layers as end points, e.g. `end= ['inception_3a/output','inception_5a/output']`. The script will alternate between the layers in the list.
- A function, `loadWithMaxSize(imagename, maxSize = 400000)`, allows you to automatically rescale images to a maximum number of pixels. This is useful to prevent out-of-memory errors.
- An example of how to do actual categorical predictions with the script.

## Windows installation

I managed to run the deepdream network with CUDA acceleration on Windows, using [this build for the Python wrappers](
https://github.com/drakh/caffe-win-python-anaconda/)

I used Anaconda 2.7, together with CUDA 7 on Windows 8.1 (all 64-bit). I needed to install protobuf using:
`conda install -c https://conda.binstar.org/dhirschfeld protobuf`
