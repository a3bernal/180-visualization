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
  
We installed and ran rviz which is the visualization for Autoware through build commands in Ubuntu. Using some sample data we created a visualization of the sample track shown here.

![Image](https://drive.google.com/uc?export=view&id=1Dw5z4BI11FbxUvhfdYO_4WYVdjiJa2iG)

### Data and Conversion
In terms of grabbing actual data, we were lucky enough to be given the thunderhill data in pcap form by students from another class also studying this course in unity. Our data that we fed into unity needed to be in the format of a PCD or point cloud data format. What we had was the thunderhill data in a PCAP file format which was a binary compression of many PCD files. To get this extraction, we used an online converter we found that someone had coded. We fixed the code up a little bit and was able to successfully do the conversion !
![Image](https://drive.google.com/uc?export=view&id=1KznTS2XIsNEJrT-Y53hQofdlYH5hjNRK)

### Integrating the Map

We decided to use a software tool called Unity to load in and improve the quality of the thunderhill race track. We were able to load in the Thunderhill Race track into Unity which including the west and east race tracks using exisisting Velodyne lidar data of the Thunder Hill Track. Since we are only working on the west trtack of the thunderhill track we trimed the racetrack to only include the west track which is about 2 miles. We were also able to add elevation data to the track to make it look as realistic as possible so that it's ready to be placed in our LGSVL simulator.
![Image](https://drive.google.com/uc?export=view&id=1feJC-iUI9h2RmhzQ9TktB5QkdAToBBnG)

![Image](https://doc-0s-a0-docs.googleusercontent.com/docs/securesc/649l0lfk0nceud27v3dfd7eh0npjh8d9/se1tg60oqu2i216oho9uulkqpgthojsb/1613374950000/10575429113603452305/18111229792978024561/1feJC-iUI9h2RmhzQ9TktB5QkdAToBBnG?e=view&authuser=1&nonce=sj1c8uhc91j8k&user=18111229792978024561&hash=elt3t449i1nmm1ash27f3ngif4hie8j3)

### Video of the Track can be found below 
[Click here to view ThundeHill track video ](https://drive.google.com/uc?export=view&id=1vtF_PLNSUShigg4YIK_W5aqYvvA_UXG8)

### Simulator

We will place our ThunderHill track from Unity and import it into the LGSVL simulator so that we can visualize how it actually looks in the simulator and we will also be able to see how our robot performs in the simulation. We decided to use this simulator since it works well with Unity and since it includes all the sensors that we need such as the lidar, odometry, IMU, etc.

