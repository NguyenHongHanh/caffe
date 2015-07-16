# Caffe for Windows

Caffe is a deep learning framework made with expression, speed, and modularity in mind.
It is developed by the Berkeley Vision and Learning Center ([BVLC](http://bvlc.eecs.berkeley.edu)) and community contributors.

This branch is for Windows using Visual Studio 2013.

# Step 1
We need following external libraries to build caffe.
- CUDA 7.0 + cuDNN
- OpenCV 2.4.8
- [Boost 1.56](http://sourceforge.net/projects/boost/files/boost-binaries/1.56.0/boost_1_56_0-msvc-12.0-64.exe/download)
- OpenBLAS (in 3rdparty)
- GFlags, GLog, Protobuf (in 3rdparty)
- LevelDB, LMDB, HDF5 (in 3rdparty)

You can download pre-built 3rd party libraries here.
https://www.dropbox.com/s/v038gymle57kn7d/3rdparty.zip?dl=0

# Step 2
Checkout if following environment variables are set.
- CUDA_PATH_V7_0
- OPENCV_HOME (like D:\dev\opencv)
- BOOST_1_56_0 (like D:\dev\boost_1_56_0)
- Path (Add D:\dev\opencv\build\x64\vc12\bin;D:\dev\caffe\3rdparty\bin)

# Step 3
Open caffe/caffe/caffe.sln and set build platform x64.
You may need some changes in additional include/library directories.
Finally, you can build caffe.
