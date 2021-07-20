+++
title = "Installing openpose on Ubuntu 20.04"
date = 2021-07-18T00:00:00

# List format.
#   0 = Simple
#   1 = Detailed
#   2 = Stream
list_format = 2
tags = ["openpose", "ubuntu"]
reading_time = false  # Show estimated reading time?
# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder.
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Right"

  # Show image only in page previews?
  preview_only = false

+++
[OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) has represented the first real-time multi-person system to jointly detect human body, hand, facial, and foot keypoints (in total 135 keypoints) on single images.

The install guide on its website, it starts with dependencies that should be installed before installing openpose. ''**DO NOT FOLLOW IT!**''. Instead, follow these steps:

1) check your Nvidia driver version in *additional drivers* page on your ubuntu. Make sure it is one of the proprietary packages.
{{< figure src="openpose1.jpg" >}}
2) Check your CUDA version using
```bash
nvcc --version
```
If CUDA is not installed, install nvidia toolkit using
```bash
sudo apt-get install nvidia-cuda-toolkit
```
and reboot.
3) Download a version of cuDNN from [here](https://developer.nvidia.com/rdp/cudnn-archive) that matches your CUDA version. Download all the .deb files for runtime and developer modes and code samples.
{{< figure src="openpose2.jpg" >}}
Install the runtime and developer ones, then install the code samples.
4) Test if cuDNN using the mnist dataset:
```bash
cp -r /usr/src/cudnn_samples_v8/ $HOME
cd  $HOME/cudnn_samples_v8/mnistCUDNN
make clean && make
chmod +x ./mnistCUDNN
```
If cuDNN is properly installed and running on your Linux system, you will see a message saying test passed!

5) Install opencv

```bash
sudo apt install libopencv-dev python3-opencv
```

6) Install and configure gcc version 8 as the default using info from this [link](https://linuxize.com/post/how-to-install-gcc-on-ubuntu-20-04/) . Check the gcc version and make sure it is version 8.

7)Now, clone openpose from the github
```bash
git clone https://github.com/CMU-Perceptual-Computing-Lab/openpose
```
8) Install OpenPose dependencies by running the shell script:
```bash
cd openpose\scripts\ubuntu
chmod +x install_deps.sh
sudo ./install_deps.sh
```
This will install all the dependencies except caffe. caffe source code is already in openpose ``3rdparty`` folder. When you build openpose, caffe will be installed.

9) Configure and make the build for OpenPose:
```bash
cd {OpenPose_folder}
mkdir build/
cd build/
cmake-gui ..
```
select the configs you want. Make sure to check build caffe, use cuDNN and openCV. Hit 'Configure' and then 'Generate'. Then close cmake.

10) Build OpenPose
```bash
cd build/
make -j5
```
11) Now, you can run a demo using the following code:
```bash
cd ..
./build/examples/openpose/openpose.bin --video examples/media/video.avi
```
