.. Copyright 2016 The Cartographer Authors

.. Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

..      http://www.apache.org/licenses/LICENSE-2.0

.. Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

============
Cartographer
============

|build| |docs|

Purpose
=======

`Cartographer`_ is a system that provides real-time simultaneous localization
and mapping (`SLAM`_) in 2D and 3D across multiple platforms and sensor
configurations.

|video|

.. _Cartographer: https://github.com/googlecartographer/cartographer
.. _SLAM: https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping

Getting started
===============

* Learn to use Cartographer at `our Read the Docs site`_.
* Please join the `mailing list`_ and ask questions.

.. _our Read the Docs site: https://google-cartographer.readthedocs.io
.. _mailing list: https://groups.google.com/forum/#!forum/google-cartographer

Contributing
============

You can find information about contributing to Cartographer at `our Contribution
page`_.

.. _our Contribution page: https://github.com/googlecartographer/cartographer/blob/master/CONTRIBUTING.md

.. |build| image:: https://travis-ci.org/googlecartographer/cartographer.svg?branch=master
    :alt: Build Status
    :scale: 100%
    :target: https://travis-ci.org/googlecartographer/cartographer
.. |docs| image:: https://readthedocs.org/projects/google-cartographer/badge/?version=latest
    :alt: Documentation Status
    :scale: 100%
    :target: https://google-cartographer.readthedocs.io/en/latest/?badge=latest
.. |video| image:: https://j.gifs.com/wp3BJM.gif
    :alt: Cartographer 3D SLAM Demo
    :scale: 100%
    :target: https://youtu.be/DM0dpHLhtX0
    
Dependencies:

sudo apt-get install -y google-mock libboost-all-dev  libeigen3-dev libgflags-dev libgoogle-glog-dev liblua5.2-dev libprotobuf-dev  libsuitesparse-dev libwebp-dev ninja-build protobuf-compiler python-sphinx  ros-indigo-tf2-eigen libatlas-base-dev libsuitesparse-dev liblapack-dev

Ceres-solver:

cd ~/catkin_ws

git clone https://github.com/hitcm/ceres-solver-1.11.0.git

mkdir -p ceres-solver-1.11.0/build

cd ceres-solver-1.11.0/build

cmake ..

make 

sudo make install

Google Cartographer:

cd ~/catkin_ws

git clone https://github.com/hitcm/cartographer.git

mkdir -p cartographer/build

cd cartographer/build

cmake .. -G Ninja

ninja

ninja test

sudo ninja install

Google Cartographer For ROS:

Rplidar For ROS:

cd ~/catkin_ws/src

https://github.com/robopeak/rplidar_ros

cd ~/catkin_ws

catkin_make



