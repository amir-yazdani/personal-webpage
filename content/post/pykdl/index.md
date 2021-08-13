+++
title = "Installing pykdl_utils on ROS"
date = 2019-09-16T00:00:00

# List format.
#   0 = Simple
#   1 = Detailed
#   2 = Stream
list_format = 2
tags = ["pykdl", "kdl", "ROS", "kinetic", "melodic", "noetic", "ubuntu", "16.04", "18.04", "20.04"]
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
# Installing Guide :
## Python 2 for Ubuntu 16.04/18.04 with ROS Kinetic/Melodic
1) move to your catkin workspace
```bash
cd ~/catkin_ws/src/
```
2) clone the `hrl_kdl` repository
```bash
git clone https://github.com/gt-ros-pkg/hrl-kdl.git
```
3) install `pykd_utils`
```bash
cd hrl-kdl/pykdl_utils
python setup.py build
sudo python setup.py install
```
4) install `hrl_geom`
```bash
cd ~/catkin_ws/src/hrl-kdl/hrl_geom/
python setup.py build
sudo python setup.py install
```
5) install `urdf_parser` and `urdfdom-py`
```bash
sudo apt-get install ros-<ROS distibution>-urdf-parser-plugin
sudo apt-get install ros-<ROS distibution>-urdfdom-py
```
6) build the catkin workspace
```bash
cd ~/catkin_ws
catkin build
```
## Python 3 for Ubuntu 20.04 with ROS Noetic
1) move to your catkin workspace
```bash
cd ~/catkin_ws/src/
```
2) clone the `hrl_kdl` repository
```bash
git clone https://github.com/amir-yazdani/hrl-kdl.git
```
3) checkout to the noetic-devel branch
```bash
cd hrl-kdl
git checkout noetic-devel
```
4) install `pykd_utils`
```bash
cd pykdl_utils
python3 setup.py build
sudo python3 setup.py install
```
5) install `hrl_geom`
```bash
cd ~/catkin_ws/src/hrl-kdl/hrl_geom/
python3 setup.py build
sudo python3 setup.py install
```
4) install `urdf_parser` and `urdfdom-py`
```bash
sudo apt-get install ros-noetic-urdf-parser-plugin
sudo apt-get install ros-noetic-urdfdom-py
```
5) build the catkin workspace
```bash
cd ~/catkin_ws
catkin build
```
