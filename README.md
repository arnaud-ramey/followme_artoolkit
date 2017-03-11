# followme_artoolkit

[![Build Status](https://travis-ci.org/arnaud-ramey/followme_artoolkit.svg)](https://travis-ci.org/arnaud-ramey/followme_artoolkit)

followme_artoolkit is used to follow a moving goal identified by its ARToolkit tag.

How to install
==============

Dependencies from sources
-------------------------

Dependencies handling is based on the [wstool](http://wiki.ros.org/wstool) tool.
Run the following instructions:

```bash
$ sudo apt-get install python-wstool
$ roscd ; cd src
$ wstool init
$ wstool merge `rospack find followme_artoolkit`/dependencies.rosinstall
$ wstool update
```

Dependencies included in the Ubuntu packages
--------------------------------------------

Please run the ```rosdep``` utility:

```bash
$ sudo apt-get install python-rosdep
$ sudo rosdep init
$ rosdep install followme_artoolkit --ignore-src
```

Build package with Catkin
-------------------------

```bash
$ catkin_make --only-pkg-with-deps followme_artoolkit
```
