# Visuzlization of Lidar Point Cloud and Radar Point cloud of Nuscenes Mini Data Set 

Hi, I am Ankit Verma, graduate student at CU ICAR. This repository enables you to visualize and get started with NuScene dataset.

# Requirements and Dependencies

  - Download NuScene mini dataset https://www.nuscenes.org/data/v1.0-mini.tgz
  - Download Lidarseg file https://www.nuscenes.org/data/nuScenes-lidarseg-mini-v1.0.tar.bz2
  - Download NuScene Develop kit https://github.com/nutonomy/nuscenes-devkit
  - Ubuntu 18.04
  - Jupyter notebook
  - pip3
  - python3
  - opencv
 
# Steps
Install Juypter Notebook 
```sh
$ pip3 install notebook
```
Install NuScene-devkit 
```sh
$ pip3 install nuscene-devkit
```
Launch Jupyternotebook
```sh
$ python -m notebook
```

# Visualize a random image from the dataset
run the file visualize_random_image and give the correct path of sample folder which you want to visualize <br />
The algorithm will select a random file and display a new image eachtime you run the code
![Visualizing a random image from CAM_FRONT](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_image.jpg)

![Visualizing a random image from CAM_FRONT](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_image2.jpg)

# Visualize Lidar PCD from the dataset
The Lidar PCD is a nx4 matric that stores x y z intensity

![Visualizing Lidar PCD](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_lidarpcd.jpg)

You can colorize the points based on the following 3 Parameters
- Height of the points
- Intesity of the points
- Semantic label of the points

We will visualize each one of them below
- Heights of the points
To get this plot run the file lidarpcd_height
![Visualizing Lidar PCD_colorize_height](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_height.jpg)
- Intensity of the points
To get this plot run the file lidarpcd_intensity
![Visualizing Lidar PCD_colorize_intensity](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_intensity.jpg)
- Semantic label of the points
To get this plot run the file lidarpcd_semantic
![Visualizing Lidar PCD_colorize_semantic](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_semantic.jpg)

# Visualize Radar PCD from the dataset
The Radar PCD is a nx18 matric that stores x y z dyn_prop id rcs vx vy vx_comp vy_comp is_quality_valid ambig_state x_rms y_rms invalid_state pdh0 vx_rms vy_rms <br />
To know more visit https://github.com/nutonomy/nuscenes-devkit/blob/5325d1b400950f777cd701bdd5e30a9d57d2eaa8/python-sdk/nuscenes/utils/data_classes.py#L259:1

You can colorize the points based on various parameter. We will explore the following
- height of the points
- velocity of the points
We will visualize each one of them below
- Heights of the points
![Visualizing_Radar_pcd_height](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/radarpcd_height.jpg)

- Velocity of the points
for this we will first calculate the resultant velocity of the point

![Visualizing](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/radarpcd_velocity.jpg)

# Ploting Lidar PCD and Radar PCD on an image
For this we will use the NuScene Devkit. <br /> Run the file Plot_PCD_to_Image.

-Ploting Lidar PCD to an image
![Visualizing](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidar_image.jpg)

-Ploting Radar PCD to an image
![Visualizing](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/radar_image.jpg)

# license
Copyright (C) 2021 Ankit Verma

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/

