# Visuzlization of Nuscenes Mini Data Set 

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
run the file visualize_random_image and give the correct path of sample folder which you want to visualize
The algorithm will select a random file and display a new image eachtime you run the code
![Visualizing a random image from CAM_FRONT](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_image.jpg)

![Visualizing a random image from CAM_FRONT](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_image2.jpg)

# Visualize Lidar PCD from the dataset
The Lidar PCD is a nx4 matric that stores x y z intensity

![Visualizing Lidar PCD](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/visualize_lidarpcd.jpg)

You can colorize the points based on the following 3 infromation
- Height of the points
To get this plot run the file lidarpcd_height
![Visualizing Lidar PCD](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_height.jpg)
- Intensity of the points
To get this plot run the file lidarpcd_intensity
![Visualizing Lidar PCD](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_intensity.jpg)
- Semantic label of the points
To get this plot run the file lidarpcd_semantic
![Visualizing Lidar PCD](https://github.com/ankitcivic/Visualize_NuScene_dataset/blob/main/images/lidarpcd_semantic.jpg)
