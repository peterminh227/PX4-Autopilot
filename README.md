# PX4 Drone Autopilot

[![Releases](https://img.shields.io/github/release/PX4/PX4-Autopilot.svg)](https://github.com/PX4/PX4-Autopilot/releases) [![DOI](https://zenodo.org/badge/22634/PX4/PX4-Autopilot.svg)](https://zenodo.org/badge/latestdoi/22634/PX4/PX4-Autopilot)

[![Nuttx Targets](https://github.com/PX4/PX4-Autopilot/workflows/Nuttx%20Targets/badge.svg)](https://github.com/PX4/PX4-Autopilot/actions?query=workflow%3A%22Nuttx+Targets%22?branch=master) [![SITL Tests](https://github.com/PX4/PX4-Autopilot/workflows/SITL%20Tests/badge.svg?branch=master)](https://github.com/PX4/PX4-Autopilot/actions?query=workflow%3A%22SITL+Tests%22)

[![Slack](/.github/slack.svg)](https://join.slack.com/t/px4/shared_invite/zt-si4xo5qs-R4baYFmMjlrT4rQK5yUnaA)

This repository holds the [PX4](http://px4.io) flight control solution for drones, with the main applications located in the [src/modules](https://github.com/PX4/PX4-Autopilot/tree/master/src/modules) directory. It also contains the PX4 Drone Middleware Platform, which provides drivers and middleware to run drones.

PX4 is highly portable, OS-independent and supports Linux, NuttX and MacOS out of the box.

* Official Website: http://px4.io (License: BSD 3-clause, [LICENSE](https://github.com/PX4/PX4-Autopilot/blob/master/LICENSE))
* [Supported airframes](https://docs.px4.io/master/en/airframes/airframe_reference.html) ([portfolio](http://px4.io/#airframes)):
  * [Multicopters](https://docs.px4.io/master/en/frames_multicopter/)
  * [Fixed wing](https://docs.px4.io/master/en/frames_plane/)
  * [VTOL](https://docs.px4.io/master/en/frames_vtol/)
  * [Autogyro](https://docs.px4.io/master/en/frames_autogyro/)
  * [Rover](https://docs.px4.io/master/en/frames_rover/)
  * many more experimental types (Blimps, Boats, Submarines, High altitude balloons, etc)
* Releases: [Downloads](https://github.com/PX4/PX4-Autopilot/releases)


## Building a PX4 based drone, rover, boat or robot

The [PX4 User Guide](https://docs.px4.io/master/en/) explains how to assemble [supported vehicles](https://docs.px4.io/master/en/airframes/airframe_reference.html) and fly drones with PX4.
See the [forum and chat](https://docs.px4.io/master/en/#support) if you need help!


## Changing code and contributing

This [Developer Guide](https://docs.px4.io/master/en/development/development.html) is for software developers who want to modify the flight stack and middleware (e.g. to add new flight modes), hardware integrators who want to support new flight controller boards and peripherals, and anyone who wants to get PX4 working on a new (unsupported) airframe/vehicle.

Developers should read the [Guide for Contributions](https://docs.px4.io/master/en/contribute/).
See the [forum and chat](https://dev.px4.io/master/en/#support) if you need help!


### Weekly Dev Call

The PX4 Dev Team syncs up on a [weekly dev call](https://dev.px4.io/master/en/contribute/#dev_call).

> **Note** The dev call is open to all interested developers (not just the core dev team). This is a great opportunity to meet the team and contribute to the ongoing development of the platform. It includes a QA session for newcomers. All regular calls are listed in the [Dronecode calendar](https://www.dronecode.org/calendar/).


## Maintenance Team

  * Project: Founder
    * [Lorenz Meier](https://github.com/LorenzMeier)
  * Architecture
    * [Daniel Agar](https://github.com/dagar)
  * [Dev Call](https://github.com/PX4/PX4-Autopilot/labels/devcall)
    * [Ramon Roche](https://github.com/mrpollo)
  * Communication Architecture
    * [Beat Kueng](https://github.com/bkueng)
    * [Julian Oes](https://github.com/JulianOes)
  * UI in QGroundControl
    * [Gus Grubba](https://github.com/dogmaphobic)
  * [Multicopter Flight Control](https://github.com/PX4/PX4-Autopilot/labels/multicopter)
    * [Mathieu Bresciani](https://github.com/bresch)
  * [Multicopter Software Architecture](https://github.com/PX4/PX4-Autopilot/labels/multicopter)
    * [Matthias Grob](https://github.com/MaEtUgR)
  * [VTOL Flight Control](https://github.com/PX4/PX4-Autopilot/labels/vtol)
    * [Roman Bapst](https://github.com/RomanBapst)
  * [Fixed Wing Flight Control](https://github.com/PX4/PX4-Autopilot/labels/fixedwing)
    * [Roman Bapst](https://github.com/RomanBapst)
  * OS / NuttX
    * [David Sidrane](https://github.com/davids5)
  * Driver Architecture
    * [Daniel Agar](https://github.com/dagar)
  * Commander Architecture
    * [Julian Oes](https://github.com/julianoes)
  * [UAVCAN](https://github.com/PX4/PX4-Autopilot/labels/uavcan)
    * [Daniel Agar](https://github.com/dagar)
  * [State Estimation](https://github.com/PX4/PX4-Autopilot/issues?q=is%3Aopen+is%3Aissue+label%3A%22state+estimation%22)
    * [Paul Riseborough](https://github.com/priseborough)
  * Vision based navigation and Obstacle Avoidance
    * [Markus Achtelik](https://github.com/markusachtelik)
  * RTPS/ROS2 Interface
    * [Nuno Marques](https://github.com/TSC21)

See also [maintainers list](https://px4.io/community/maintainers/) (px4.io) and the [contributors list](https://github.com/PX4/PX4-Autopilot/graphs/contributors) (Github).

## Supported Hardware

This repository contains code supporting Pixhawk standard boards (best supported, best tested, recommended choice) and proprietary boards.

### Pixhawk Standard Boards
  * FMUv6X and FMUv6U (STM32H7, 2021)
    * Various vendors will provide FMUv6X and FMUv6U based designs Q3/2021
  * FMUv5 and FMUv5X (STM32F7, 2019/20)
    * [Pixhawk 4 (FMUv5)](https://docs.px4.io/master/en/flight_controller/pixhawk4.html)
    * [Pixhawk 4 mini (FMUv5)](https://docs.px4.io/master/en/flight_controller/pixhawk4_mini.html)
    * [CUAV V5+ (FMUv5)](https://docs.px4.io/master/en/flight_controller/cuav_v5_plus.html)
    * [CUAV V5 nano (FMUv5)](https://docs.px4.io/master/en/flight_controller/cuav_v5_nano.html)
    * [Auterion Skynode (FMUv5X)](https://docs.px4.io/master/en/flight_controller/auterion_skynode.html)
  * FMUv4 (STM32F4, 2015)
    * [Pixracer](https://docs.px4.io/master/en/flight_controller/pixracer.html)
    * [Pixhawk 3 Pro](https://docs.px4.io/master/en/flight_controller/pixhawk3_pro.html)
  * FMUv3 (STM32F4, 2014)
    * [Pixhawk 2](https://docs.px4.io/master/en/flight_controller/pixhawk-2.html)
    * [Pixhawk Mini](https://docs.px4.io/master/en/flight_controller/pixhawk_mini.html)
    * [CUAV Pixhack v3](https://docs.px4.io/master/en/flight_controller/pixhack_v3.html)
  * FMUv2 (STM32F4, 2013)
    * [Pixhawk](https://docs.px4.io/master/en/flight_controller/pixhawk.html)
    * [Pixfalcon](https://docs.px4.io/master/en/flight_controller/pixfalcon.html)

### Manufacturer and Community supported
  * [Holybro Durandal](https://docs.px4.io/master/en/flight_controller/durandal.html)
  * [Hex Cube Orange](https://docs.px4.io/master/en/flight_controller/cubepilot_cube_orange.html)
  * [Hex Cube Yellow](https://docs.px4.io/master/en/flight_controller/cubepilot_cube_yellow.html)
  * [Airmind MindPX V2.8](http://www.mindpx.net/assets/accessories/UserGuide_MindPX.pdf)
  * [Airmind MindRacer V1.2](http://mindpx.net/assets/accessories/mindracer_user_guide_v1.2.pdf)
  * [Bitcraze Crazyflie 2.0](https://docs.px4.io/master/en/complete_vehicles/crazyflie2.html)
  * [Omnibus F4 SD](https://docs.px4.io/master/en/flight_controller/omnibus_f4_sd.html)
  * [Holybro Kakute F7](https://docs.px4.io/master/en/flight_controller/kakutef7.html)
  * [Raspberry PI with Navio 2](https://docs.px4.io/master/en/flight_controller/raspberry_pi_navio2.html)

Additional information about supported hardware can be found in [PX4 user Guide > Autopilot Hardware](https://docs.px4.io/master/en/flight_controller/).

## Project Roadmap

A high level project roadmap is available [here](https://github.com/orgs/PX4/projects/25).
## Minh's edit - compling PX4 firmware
``
sudo apt-get install -y gcc-arm-none-eabi
``
## Running offboard example from px4 website

```
cd PX4-Autopilot
sudo git checkout v1.10.2 
git submodule update --init --recursive
```
```
cd ..
chmod -R 777 PX4-Autopilot/
```
Install tools & dependencies
```
bash ./PX4-Autopilot/Tools/setup/ubuntu.sh
sudo apt install -y ninja-build exiftool python-argparse python-empy python-toml python-numpy python-yaml python-dev python-pip ninja-build protobuf-compiler libeigen3-dev genromfs xmlstarlet libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
sudo pip3 install --user pandas jinja2 pyserial cerberus pyulog numpy toml pyquaternion  
```
Edit an error in v1.10.2 in
```
gedit ./PX4-Autopilot/Tools/sitl_gazebo/include/gazebo_opticalflow_plugin.h
```
please change as following
```
#define HAS_GYRO true (make TRUE lowercase).
```
```
cd PX4-Autopilot
make px4_sitl_default gazebo
```
A usefull script to add paths mavros & SITL: launch_common.sh
```
#!/bin/bash

px4_dir=$(pwd)/../PX4-Autopilot

source $px4_dir/Tools/setup_gazebo.bash $px4_dir $px4_dir/build/px4_sitl_default

export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$px4_dir
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$px4_dir/Tools/sitl_gazebo

```
and running mavros & SITL
```
#!/bin/bash

source ./launch-common.sh
# mavros
gnome-terminal -- /bin/sh -c 'roslaunch mavros px4.launch fcu_url:="udp://:14540@127.0.0.1:14557";exec bash'
# px4-sitl
gnome-terminal -- /bin/sh -c 'source /home/samurai/shell_script/launch-common.sh;roslaunch px4 posix_sitl.launch;exec bash'

```
Some useful links
[[1]](https://programs.team/px4-uav-gazebo-simulation-to-track-moving-objects.html)
[[2]](https://darienmt.com/autonomous-flight/2018/11/25/px4-sitl-ros-example.html)


