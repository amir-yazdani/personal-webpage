+++
title = "Installing pykdl_utils on ROS kinetic, Ubuntu 16.04"
date = 2019-09-16T00:00:00

# List format.
#   0 = Simple
#   1 = Detailed
#   2 = Stream
list_format = 2
tags = ["pykdl", "kdl", "ros", "kinetics", "ubuntu"]
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
1) clone the `hrl_kdl` repository
```bash
git clone https://github.com/gt-ros-pkg/hrl-kdl.git
```
2) install `pykd_utils`
```bash
cd hrl-kdl/pykdl_utils
python setup.py build
sudo python setup.py install
```
3) install `hrl_geom`
```bash
cd ~/catkin_ws/src/hrl-kdl/hrl_geom/
python setup.py build
sudo python setup.py install
```
4) install `urdf_parser` and `urdfdom-py`
```bash
sudo apt-get install ros-kinetic-urdf-parser-plugin
sudo apt-get install ros-kinetic-urdfdom-py
```
5) building the catkin workspace
```bash
cd ~/catkin_ws
catkin build
```
