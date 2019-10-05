# deeplab_ros

## Install

$ cd (YOUR_CATKIN_WORKSPACE)/src

$ git clone https://github.com/Taka-Kazu/deeplab_ros

$ cd deeplab_ros

$ git submodule update --init --depth=1

## Network weight
place cityscape weight to ./deeplab_ros/scripts/

## Run
$ roslaunch deeplab_ros deeplab_ros.launch

### subscribied topic
- /usb_cam/image_raw (sensor_msgs/Image)

### published topics
- /deeplab/segmented_image (sensor_msgs/Image)
  - segmentation map only
- /deeplab/masked_image (sensor_msgs/Image)
  - rgb image masked by segmentation map
