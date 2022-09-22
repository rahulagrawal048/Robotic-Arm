# Click to watch the video

<a href="http://www.youtube.com/watch?feature=player_embedded&v=JX__0Y76WpM" target="_blank">
 <img src="https://img.youtube.com/vi/JX__0Y76WpM/0.jpg" alt="Watch the video" width="480" height="360" border="10" />
</a>



Launch realsense:

roslaunch realsense2_camera rs_camera.launch align_depth:=true

Launch rx200 arm:

roslaunch interbotix_sdk arm_run.launch robot_name:=rx200 use_time_based_profile:=true gripper_operating_mode:=pwm
