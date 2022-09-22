# Robotic Arm for Manipulation

The algorithmic design of a 5 degree-of-freedom robotic arm for manipulation.
The objective is to detect blocks, stacked or unstacked in a workspace using a RGB-D camera,
and apply path planning and kinematics to a robotic arm to pick and place the blocks. 
3D calibration was successfully performed for transformation between image and world coordinates.
Block detection was implemented and blocks of various col- ors and two sizes were detected along 
with their centroids and orientation. Inverse Kinematics and motion planning was implemented to 
grab and place blocks according to the task.

# Click to watch the video

<a href="http://www.youtube.com/watch?feature=player_embedded&v=JX__0Y76WpM" target="_blank">
 <img src="https://img.youtube.com/vi/JX__0Y76WpM/0.jpg" alt="Watch the video" width="480" height="360" border="10" />
</a>

# Launching ROS drivers

Launch realsense:

roslaunch realsense2_camera rs_camera.launch align_depth:=true

Launch rx200 arm:

roslaunch interbotix_sdk arm_run.launch robot_name:=rx200 use_time_based_profile:=true gripper_operating_mode:=pwm
