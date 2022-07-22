# Ai-robotics-week-2-tasks
**Task 1: Installing Ubunto and ROS in a virtual machine**  

**1. Install Oracle VM virtual box: https://www.virtualbox.org/wiki/Downloads**

choose the latest version and click on Windows Hosts 

![image](https://user-images.githubusercontent.com/108147030/180487488-dcfe3d5d-ff50-417b-8be7-dbb464b2acc8.png)

**2. Download Ubuntu 16.04.7 LTS (Xenial Xerus): https://releases.ubuntu.com/16.04/**

Choose 64-bit PC (AMD64) desktop image

![image](https://user-images.githubusercontent.com/108147030/180487843-c348c078-a376-4c49-b17f-3ef900461afd.png)

**3. Steps on installing Ubunto with ROS on the virtual machine:**

  1) From the Virtual box software, click on NEW.
  
  ![image](https://user-images.githubusercontent.com/108147030/180488271-dcc03e6b-ce42-49a8-ac4c-59909567d162.png)

  2) Choose the name and destination folder after that click on Next: 
  
  ![image](https://user-images.githubusercontent.com/108147030/180488658-8338fafa-5aa5-4089-aa31-28d8b7765748.png)
  
  3) Choose the maximum amount of memory from the green bar (do not pass through the green bar to the orange/red) then click Next:
  
![image](https://user-images.githubusercontent.com/108147030/180491262-b0bab43a-12d2-4657-bb6d-0759e8ae4767.png)
    
  4) Keep clicking Next until you get to the virtual hard disk size, its recommend to have it at 32GB then click on create:
  
  ![image](https://user-images.githubusercontent.com/108147030/180489852-35507ef6-acc8-4874-a480-784006d84575.png)
  
  5) Now click on your virtual machine then click on settings:
    
![image](https://user-images.githubusercontent.com/108147030/180491341-404aa885-78c6-488e-9b0e-54db03b0ca12.png)

  6) From settings go to system > processor and choose the maximum amout of CPU with only the green bar:
  
 ![image](https://user-images.githubusercontent.com/108147030/180490984-8c9242e9-004c-4412-83af-34dd1a61ce0a.png)
 
  7) Go to display settings and choose the maximum amount of video memory:

  ![image](https://user-images.githubusercontent.com/108147030/180491576-bb3a1ae2-bbd4-4829-8dda-ebc5c8e684f2.png)
  
  8) Go to storage settings and click on the "Empty" CD and then from Attributes click on the CD symbol and click on "choose a disk file..." from there you can choose the ISO file that is Ubunto 16.04 that was downloaded before:

![image](https://user-images.githubusercontent.com/108147030/180494397-14baa016-1d5d-4e56-8ca6-92c44f00dbbe.png)

  9) Finally you can now run your virtual machine and follow through the installation guide for Ubunto, after installing Ubunto, open terminal and run each of the following commands to install ROS: 
  
 

    i. sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    
    ii. sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
    
    iii. sudo apt-get update
    
    iv. sudo apt-get install ros-kinetic-desktop-full
    
    v. apt-cache search ros-kinetic
    
    vi. echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
    
    vii. source ~/.bashrc
    
    viii. sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
    
    ix. sudo apt install python-rosdep
    
    x. sudo rosdep init

    xi. rosdep update

    xii. sudo apt-get install ros-noetic-catkin

![image](https://user-images.githubusercontent.com/108147030/180494818-777f7709-ad4c-4305-8e73-64cc4577baa9.png)


