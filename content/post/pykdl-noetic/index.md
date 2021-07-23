+++
title = "Installing pykdl_utils on ROS Noetic, Ubuntu 20.04"
date = 2021-07-21T00:00:00

# List format.
#   0 = Simple
#   1 = Detailed
#   2 = Stream
list_format = 2
tags = ["pykdl", "kdl", "ROS", "noetic", "ubuntu", "python3", "python"]
reading_time = false  # Show estimated reading time?
# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder.
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""

  # Show image only in page previews?
  preview_only = false

+++
1) Clone the `hrl_kdl` repository in your catkin-ws folder
```bash
cd ~/catkin_ws/src/
git clone https://github.com/amir-yazdani/hrl-kdl.git
```
2) Checkout to the noetic-devel branch
```bash
cd hrl-kdl
git checkout noetic-devel
```
3) Install `pykd_utils`
```bash
cd hrl-kdl/pykdl_utils
python3 setup.py build
sudo python3 setup.py install
```
3) Install `hrl_geom`
```bash
cd ~/catkin_ws/src/hrl-kdl/hrl_geom/
python3 setup.py build
sudo python3 setup.py install
```
4) Install `urdf_parser` and `urdfdom-py`
```bash
sudo apt-get install ros-noetic-urdf-parser-plugin
sudo apt-get install ros-noetic-urdfdom-py
```
5) Build the catkin workspace
```bash
cd ~/catkin_ws
catkin build
```
