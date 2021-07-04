# Turtlebot3-with-SLAM
Use Turtlebot3 with SLAM approach to create and save a map.
http://turtlebot3.robotis.com/

### **PC Setup**

**1- Download and Install Ubuntu on PC**

**2- Install ROS 1 on Remote PC**

Open the terminal and enter below commands one at a time.

`$ sudo apt update`

`$ sudo apt upgrade`

`$ wget https://raw.githubusercontent.com/ROBOTIS-GIT/robotis_tools/master/install_ros_melodic.sh`

`$ chmod 755 ./install_ros_melodic.sh` 

`$ bash ./install_ros_melodic.sh`

**3- Install Dependent ROS 1 Packages**

`$ sudo apt-get install ros-melodic-joy ros-melodic-teleop-twist-joy \`
  `ros-melodic-teleop-twist-keyboard ros-melodic-laser-proc \`
  `ros-melodic-rgbd-launch ros-melodic-depthimage-to-laserscan \`
  `ros-melodic-rosserial-arduino ros-melodic-rosserial-python \`
  `ros-melodic-rosserial-server ros-melodic-rosserial-client \`
  `ros-melodic-rosserial-msgs ros-melodic-amcl ros-melodic-map-server \`
  `ros-melodic-move-base ros-melodic-urdf ros-melodic-xacro \`
  `ros-melodic-compressed-image-transport ros-melodic-rqt* \`
  `ros-melodic-gmapping ros-melodic-navigation ros-melodic-interactive-markers`

**4- Install TurtleBot3 Packages**

`$ sudo apt-get install ros-melodic-dynamixel-sdk`

`$ sudo apt-get install ros-melodic-turtlebot3-msgs`

`$ sudo apt-get install ros-melodic-turtlebot3`


**5- Set TurtleBot3 Model Name**

In case of TurtleBot3 Burger

`$ echo "export TURTLEBOT3_MODEL=burger" >> ~/.bashrc`

In case of TurtleBot3 Waffle Pi

`$ echo "export TURTLEBOT3_MODEL=waffle_pi" >> ~/.bashrc`


**6- Network Configuration**

*  Connect PC to a WiFi device and find the assigned IP address with the command below.

`$ ifconfig`

*  Open the file and update the ROS IP settings with the command below.

`$ nano ~/.bashrc`

*  Press Ctrl+END or Alt+/ to move the cursor to the end of line.
Modify the address of localhost in the ROS_MASTER_URI and ROS_HOSTNAME with the IP address acquired from the above terminal window.

* Source the bashrc with below command.

`$ source ~/.bashrc`
