# ROS-powered EduKit Bot

[![Snap Status](https://build.snapcraft.io/badge/kyrofa/edukit_bot.svg)](https://build.snapcraft.io/user/kyrofa/edukit_bot)

This is a ROS workspace that allows for teleoperation of the
[EduKit #3, the robotics kit][1], all from ROS. This was written to accompany
the [Your First Robot][2] series written by Kyle Fazzari.

It can be installed with:

    $ sudo snap install edukit-bot-kyrofa

Note that the `joystick` interface is needed for access to the gamepad, and the
`physical-memory-control` interface is needed for access to GPIO. Both of these
interfaces must be connected before this snap will function:

    $ sudo snap connect edukit-bot-kyrofa:joystick
    $ sudo snap connect edukit-bot-kyrofa:physical-memory-control

[1]: http://camjam.me/?page_id=1035
[2]: https://kyrofa.com/posts/your-first-robot-a-beginner-s-guide-to-ros-and-ubuntu-core-1-5
