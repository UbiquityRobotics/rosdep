# ubiquity rosdep
rosdep overlays for Ubiquity Robotics packages

## What is rosdep? Why do we need an overlay?
rosdep is the system ROS uses for defining system dependancies.
Many common dependancies are already supported in the [standard rosdep][1].
Some of the raspberry pi deps used by raspicam are not declared there, 
so we define them in this 'overlay'.

You can add this overlay to your system creating the file: 
`/etc/ros/rosdep/sources.list.d/30-ubiquity.list` and add this to it.

```
yaml https://raw.githubusercontent.com/UbiquityRobotics/rosdep/master/raspberry-pi.yaml
```

[1]: https://github.com/ros/rosdistro/tree/master/rosdep

