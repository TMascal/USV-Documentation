# Sensor Types
***

Sensors and Sensor Selection are critical steps in the design of a Robotics System. They often determine how a problem is 
approached because of their availability and cost. Often times there are multiple approaches to the same problem, i.e. 
Using a camera (Telsa Self Driving) or a radar (Waymo Self Driving) for navigation tasks. Cameras are less expensive and 
more available, but may suffer in low disability conditions. Here is an [article](https://research.contrary.com/deep-dive/tesla-waymo-and-the-great-sensor-debate) on the debate on sensor selection 
between Tesla and Waymo.

Regardless of how you approach your problem, there will be trade offs that need to be carefully considered. You will 
have a limited budget, limited time, limited knowledge, and a defined scope. 

>*The greatest time investment you can make is a well thought out system plan.*

## Sensor System Planning
Your system plan should do the following
1. Outline the Requirements from the Customer
2. Connect a possible solution to the Requirements
3. Define your interfaces from your sensors to the Software.
   * What data will you be expecting to get?
4. Compare against the cost of the sensors you need.
5. Estimate the Compute Cost of the Data Incoming.
6. Ensure your sensor suite complies with the computing power.

___
# Navigation Sensor Options

## Imaging Sensors
### Cameras
#### Standard Cameras
> Typical Domain: Ground, Air, Surface, and Subsurface
#### Spectral Cameras
> Typical Domain: Ground, Air, Surface, and Subsurface
#### Stereo Cameras
> Typical Domain: Ground, Air, Surface, and Subsurface

## Ranging Sensors
### LiDAR
> Typical Domain: Ground, Air, Surface, and limited Subsurface
### Radar
> Typical Domain: Ground, Air, and Surface
### Ultrasonic Range Finder
> Typical Domain: Ground, Air, and Surface
### Echosounder
> Typical Domain: Surface, and Subsurface
### Scanning Sonar
> Typical Domain: Surface, and Subsurface
### Imaging Sonar
> Typical Domain: Surface, and Subsurface

## Localizing Sensors
### GPS
> Typical Domain: Ground, Air, Surface, and limited Subsurface
### Hydrophone Array
> Typical Domain: Surface, and Subsurface
### Doppler Velocity Logger
> Typical Domain: Surface, and Subsurface

## Tilt Sensor
### AHRS
> Typical Domain: Ground, Air, Surface, and Subsurface
### IMU
> Typical Domain: Ground, Air, Surface, and Subsurface
