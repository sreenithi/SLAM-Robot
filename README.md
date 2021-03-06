# Robot Mapping
A simple robot modelled using URDF and programmed using ROS that can map the environment around it using the RTAB-Map Mapping algorithm

The ROS project consists of 2 packages, **my_robot** and **mapping**. The *my_robot* package contains the robot and world models which can be visualised in the Gazebo simulator when the package is run using the *roslaunch* command. The *mapping* package is responsible for running the rtabmap node to perform the mapping of the environment

The generated map of the environment can be downloaded from this [Google Drive link](https://drive.google.com/file/d/1BS2ZHMQ3DfcHB2GY2XRt6YWq-5GGZlvh/view?usp=sharing). Any new map generated when running the rtabmap node for mapping is saved to the mapping/db folder.

To view the existing map dowloaded from the link in the database viewer, run the command<br>
`rtabmap-databaseViewer (map db location)/rtabmap.db`

The 3D model of the map can be viewed using the **Edit -> View 3D Map** option from the *rtabmap-databaseViewer*. Alternatively the 3D Point Cloud Data file (.pcd file) can be downloaded from [this link](https://drive.google.com/file/d/1SlwNu3WojOs4svx0SMrkxtV3zSPhAN7Q/view?usp=sharing). Once downloaded it can be viewed using the *pcl_viewer*. The top and side views of the map are also available as .jpg files in the *mapping/db* folder.


## Nodes
* rtabmap (Mapping)
* rtabmap (Localisation)

  
## ROS and Ubuntu version used
ROS Kinetic in Ubuntu 16.04
