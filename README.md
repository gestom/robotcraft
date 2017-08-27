# Robotcraft 2017
## Visual Navigation in Changing Environments

### Demo 1: Dealing with shadows

### Demo 2: Map-and-replay navigation

Make your usb camera work:
1. Clone and compile the usb_cam ROS driver: `git clone https://github.com/ros-drivers/usb_cam.git`
1. Run the camera node: `roslaunch usb_cam usb_cam-test.launch`

Make the `stroll_bearnav` package work:
1. Clone and compile the stroll_bearnav package: `git clone https://github.com/gestom/stroll_bearnav.git`
1. Run it: `roslaunch stroll_bearnav stroll-core.launch`
1. Check the image features: `rosrun image_view image_view image:=/image_with_features`
1. Check the system structure `rosrun rqt_graph rqt_graph`
1. Run the operator GUIs: `roslaunch stroll_bearnav stroll-gui.launch`
1. Create a map by entering its name, e.g. `A_0` in the action client `mapper` gui, clicking `Send goal` and then `Cancel goal`.
1. Load the map by entering its name in the action client `map_preprocessor` gui, clicking `Send goal`
1. Start the navigation by clicking `Send goal` in the `navigation` gui.

