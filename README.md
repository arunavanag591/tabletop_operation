# tabletop_operation
This repository performs tabletop_operation using Kinect and PCL libraries. The robot used is Baxter. Clustering and planar segmentation has been done using PCL in ROS Indigo.

Visual Demo: https://youtu.be/_suyKDMEdro

The steps to run this is:

$roscore 

$roslaunch openni_launch openni.launch (I have used a kinect xbox 360)

$rosrun tabletop_operation planar input:=/camera/depth/points (to view the planar segmentation)

$rosrun tabletop_operation cluster_euclid input:=/camera/depth/points  (to view the euclidean clustering)

The results can be viewed in rviz by running rviz through 

$rosrun rviz rviz 

Change the default topic to camera_depth_frame. Also add a Pointcloud2 topic and subscribe to /output for planar segmentation and /clusters for euclidean clustering.

Contact: 
arunava-nag.branded.me

