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

   1- download Ubuntu 16.04.7 LTS (Xenial Xerus)  [here](https://releases.ubuntu.com/16.04/)
   
   2- choose 64-bit PC (AMD64) desktop image and download 
   
   3- open the Oracle VM VirtualBox
   
   4- press New button to create virtual machine 
   
   5- enter the Name then press Next 
   
   6- memory size,Move the arrow to the end of the green line then press Next
   
   7- then you don't need to change any options just next>next>next>create
   
   8- Now you have a new virtual machine 
   
   9- open it and press start button 
   
  10- press file icone then press add then choose the file of ubuntu-16.04.7 you downloaded befor , then press start 
  
  11- then choose install Ubunto then continue>continue
  
  12- then choose the Area and continue
  
  13- then Fill in the required your name and etc then press continue
  
  14- then the Ubuntu will open!
  
 ![2](https://user-images.githubusercontent.com/64277741/179371667-b0c6f5f1-7ba7-45ec-b848-9d42226ff608.PNG)
 
   Figure (2): the Ubunto interface  
   
  ### 3- install ROS1 in Ubunto
  
