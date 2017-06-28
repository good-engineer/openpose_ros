# Using OPENPOSE Wrapper
1. Install openpose and its dependencies then enable the package by running
````
./install_openpose_and_enable_package.sh
````
2. If everything succeeds, run `catkin build`, source your workspace then:
````
roscd openpose_ros_pkg/../openpose
rosrun openpose_ros_pkg openpose_ros --image_dir examples/media/
````
3. To start the ros service run:
````
rosrun openpose_ros_pkg openpose_ros_node 
````
4. To test if the service is working run:
````
rosrun openpose_ros_pkg test_openpose_ros_service_call 
````
and subscribe to `/openpose_ros/input_image` for the input image and `/openpose_ros/detected_poses_image` for the output image