How to run this script.

1. Start Gazebo:

   1.1. Open a terminal. Enter the PX4 source code folder, namely, "~/PX4-Autopilot/".

   1.2. Run **make px4_sitl_default gazebo**
   
   `If you have any bugs, just fix it. Everything would happen when you are compiling PX4.`
   
2. Start MAVROS, namely, the communication between ROS and the Control unit of the drone (PX4).

   2.1. Open another folder and source this ROS package.

   2.2. Run **roslaunch fntsmc-ppo-ros start.launch**

3. Start control node.

   3.1 Open another folder and source this ROS package.

   3.2. Run **rosrun fntsmc-ppo-ros control_ros2.py** 
   `rosrun fntsmc-ppo-ros control_ros.py also works, but it is the old version` 

4. (Optional) Polt curve

   4.1 Open another folder and enter the folder of "plot.py"

   4.2 Run **python3 plot.py**

哎，然后这个无人机就在Gazebo环境里面就该飞起来了啊

控制效果就是自己的控制器，里面爱加啥加啥，但是目前只有外环控制。
