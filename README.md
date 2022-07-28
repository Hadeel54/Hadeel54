- 👋 Hi, I’m @Hadeel54
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- steps:
- step 1 : install ros by wrting cods in the terminal
- udo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt-get update

sudo apt-get install ros-kinetic-desktop-full

apt-cache search ros-kinetic

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

sudo apt install python-rosdep

sudo rosdep init

rosdep update
- step 2 : creat catkin file also by writing cods in tirmenal 
- sudo apt-get install ros-noetic-catkin

mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
step 3 :open a new terminal and write these cods
sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/write your name/catkin_ws/devel/setup.bash)
then 
ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch
step 4 : the arm pkg will be obened
<img width="960" alt="2022-07-28" src="https://user-images.githubusercontent.com/108948042/181589129-fef108d4-cb61-41cd-a85c-555bc74cd2e4.png">



<!---
Hadeel54/Hadeel54 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
