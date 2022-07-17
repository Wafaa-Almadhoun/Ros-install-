# Ros-install-in-Windows-10-with-64-bit-operating-system
## Table of contents
* [Introduction](#Introduction)
* [Algorithm](#Algorithm)

## Introduction
Robot Operating System (ROS or ros) is an open-source robotics middleware suite. Although ROS is not an operating system (OS) but a set of software frameworks for robot software development , the versions of :
1.	ROS 1
2.	ROS 2
3.	ROS-Industrial


Operating Systems ROS runs only on Unix servers. While ROS includes software for Ubuntu, Mac OS X, and Fedora, Gentoo, Arch Linux, and other Linux platforms


If you are working on Ubuntu, it doesn’t matter. But what for Windows people? Here we go!


To install software, you may have to satisfy the system requirements. To install ROS in windows, you need the following system requirements.


You must have a Windows 10 64-bit device


Also, it is recommended that you have at least 20GB of free space on your C:\ drive for installation and development.


 * You need virtualbox to use Ubuntu and  develop ROS projects for Windows. 
 
 ## Algorithm
 
 to downloud ROS 1 we need :
 
 1- install virtualbox 
 
 2- install Ubunto in virtualbox
 
 3- install ROS1 in Ubunto
 
   following the steps :
   
  ### 1- install virtualbox 
  
  1- download virtualbox (VirtualBox 6.1.34 )platform packages [here](https://www.virtualbox.org/wiki/Downloads) 
  
  2- choose windows hosts 
  
  3- open file and setup the program 
  
  4- you don't need to change any options just next>next>next>finish
  
  5- open the Oracle VM VirtualBox 
  
  ![1](https://user-images.githubusercontent.com/64277741/179366616-adc5c727-3d54-40de-b673-f5240ac48b65.PNG)
  
  Figure (1): the VirtualBox interface  
  
### 2- install Ubunto in virtualbox

   1- download Ubuntu 20.04.4 LTS (Focal Fossa)  [here](https://releases.ubuntu.com/20.04.4/?_ga=2.177518757.1254341069.1657984651-340755649.1657984651)
   
   2- choose 64-bit PC (AMD64) desktop image and download 
   
   3- open the Oracle VM VirtualBox
   
   4- press New button to create virtual machine 
   
   5- enter the Name then press Next 
   
   6- memory size,Move the arrow to the end of the green line then press Next
   
   7- then you don't need to change any options just next>next>next>create
   
   8- Now you have a new virtual machine 
   
   9- open it and press start button 
   
  10- press file icone then press add then choose the file of Ubuntu 20.04.4 you downloaded befor , then press start 
  
  11- then choose install Ubunto then continue>continue
  
  12- then choose the Area and continue
  
  13- then Fill in the required , your name and etc then press continue
  
  ![4](https://user-images.githubusercontent.com/64277741/179374749-b6ee0723-3c7f-4018-a371-0535f4c770b7.PNG)
  
      Figure (2): the Ubuntu loading 

  
  14- then the Ubuntu will open!
  
  ![5](https://user-images.githubusercontent.com/64277741/179374785-bf410d92-4642-4840-8672-b52cf6bfc4ea.PNG)

   Figure (3): the Ubunto interface  
   
  ### 3- install ROS1 in Ubunto
   
  1- open Ubuntu
   
     first you have to open ros wiki in ubuntu with any browser [here](http://wiki.ros.org/noetic/Installation/Ubuntu)
   
  2- open terminal // command interface
   
   ![6](https://user-images.githubusercontent.com/64277741/179374796-6e1bde79-87a5-4266-b8ed-51f063b7c747.PNG)

    Figure (4): the terminal interface 
    
 3- Enter the command to configure the machin to install the ROS on it ,copy and paste then press Enter , enter the password 
  
   
         sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
         
    
         
  4- Enter the command to open the keyserver in the machine ,copy and paste then press Enter
         
          sudo apt install curl # if you haven't already installed curl
            curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
            
      
  5- Enter the command to installation, copy and paste then press Enter
         
          sudo apt update
          
  6- Enter the command to install noetic desktop full : Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages  , then run
   
          sudo apt install ros-noetic-desktop-full
          
  7- Enter the command to install packages :There are even more packages available in ROS. 
      You can always install a specific package directly.:
          
                 sudo apt install ros-noetic-PACKAGE
          
    e.g.
          
                 sudo apt install ros-noetic-slam-gmapping
          
   8- Enter the command to environment setup , then run   
         
                 source /opt/ros/noetic/setup.bash
       
   It can be convenient to automatically source this script every time a new shell is launched. These commands will do that for you.
        
   Bash
    
                 echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
                 source ~/.bashrc
        
   zsh
    
                 echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc
                 source ~/.zshrc
    
    
    Up to now you have installed what you need to run the core ROS packages. 
    
    To create and manage your own ROS workspaces, there are various tools and requirements
    
    that are distributed separately. For example, rosinstall is a frequently used command-line
    
    tool that enables you to easily download many source trees for ROS packages with one command
    
    

         

  
