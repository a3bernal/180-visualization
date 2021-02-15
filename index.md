## DSC180


### Overview
We are developing a 3D simulation environment representative of rich real world data to reliably test and simulate robotic agents in dynamic environments. This work is important because it can help streamline the remote development process and help others visually debug and evaluate the components of the robot they are working on.To accomplish this we are using the Unity 3D game engine to replicate the3-mile Thunderhill race track and create debugging tools for others to visually evaluate their algorithms in real world scenarios.  
Additionally, we will use theLGSVL simulator to virtualize the functionality of common sensors like IMU,GPS, Odometry, and Lidar devices.  Finally, we plan on exploring the feasibil-ity of using the Autoware.AI framework to assist with localization, detection,prediction and planning computations of the robot.

### Autoware Setup

The requirements needed for Autoware:
  - CPU: An i5 is needed at the bare minimum but an i7 is recommended
  - Memory:  16GB to 32GB
  - Graphics Card: NVIDIA GTX GeForce GPU(980M or higher performance)
  - SSD: At least 30 GB
  - Alternative for GPU: Use an Nvidia Drive
  
We installed and ran Rviz which is the visualization for Autoware through build commands in Ubuntu. Using some sample data we created a visualization of the sample track shown here.

### Data and Conversion
In terms of grabbing actual data, we were lucky enough to be given the thunderhill data in pcap form by students from another class also studying this course in unity. Our data that we fed into unity needed to be in the format of a PCD or point cloud data format. What we had was the thunderhill data in a PCAP file format which was a binary compression of many PCD files. To get this extraction, we used an online converter we found that someone had coded. We fixed the code up a little bit and was able to successfully do the conversion !
![Image](src)

### Integrating the Map

### Simulator

### Demo Video
