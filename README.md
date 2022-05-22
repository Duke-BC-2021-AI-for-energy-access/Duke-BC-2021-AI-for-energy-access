## Hi there 👋

This repo contains the work of the [2021 Duke Bass Connections Team: Creating AI For Artificial Worlds](https://bassconnections.duke.edu/project-teams/creating-artificial-worlds-ai-improve-energy-access-data-2021-2022). With this team, we worked under Duke professors [Dr. Kyle Bradbury](https://ece.duke.edu/faculty/kyle-bradbury) and [Dr. Jordan Malof](https://ece.duke.edu/faculty/jordan-malof), exploring the benefit of synthetic satellite imagery (using the GP-GAN) for domain adaptation on the object detection task of energy infrastructure.

We have also culminated our team's history, work, and results on our website, which can be found at [this link](https://duke-bc-2021-ai-for-energy-access.github.io/BC-2021-AI-for-energy-access/).

Our year-long research included a variety of tasks, which can be found in repos below:

## Collecting Images

Here we collect satellite images (from the NAIP dataset) using Google Earth Engine

## [Image Augmentation](https://github.com/Duke-BC-2021-AI-for-energy-access/Image-Augmentation)

Here we perform copy-paste augmentation using real objects from our source data placed in random orientations on a white canvas (that will be input into the GP-GAN.

## [Synthetic Image Creation](https://github.com/Duke-BC-2021-AI-for-energy-access/GP-GAN)

Here, we use images and their binary masks created in the image augmentation task, as well as unlabeled background images from our target domain collected from Google Earth Engine. These are input into the GP-GAN via our scripts to create realistic synthetic. arget imagery 

## [Experiments](https://github.com/Duke-BC-2021-AI-for-energy-access/Experiments)

Here includes the scripts that we developed to run our training and testing data for several trials and domain combinations with mixed batch training. We ran these in the [repro_bass repo](https://github.com/Duke-BC-2021-AI-for-energy-access/repro_bass), which was our most active repository holding the yolov3 folder to run our experiments out of, as well as our constantly updated scripts folder.

## [Comparing Against Domain Adaptation](https://github.com/Duke-BC-2021-AI-for-energy-access/Experiments)

In order to determine the effectiveness of our technique, we tested our technique against several state-of-the-art domain adaptation techniques, including CyCADA and CycleGAN. Additionally, we tested against pixelwise methods such as GrayWorld, Histogram Matching, and Histogram Equalization. 

## [Miscellaneous Scripts](https://github.com/Duke-BC-2021-AI-for-energy-access/Miscellanous-Scripts)

Here includes code developed for data pre-processing, plotting bounding boxes on images, and more.

## [Training YOLOv3](https://github.com/Duke-BC-2021-AI-for-energy-access/repro_bass)

This repository includes scripts for training the object detection model on various platforms. There are three branches:
- **main**, for training on *pizer*
- **gaia** and **gaiav2**, for training on *gaia*
- **dcc**, for training on the Duke Computing Cluster, with Python scripts that can be used to generate SLURM batch job scripts
Note that cloning the above `repro_bass` repository does not work out of the box. One would need to download various files (mostly `.pt` and `.data` files in the `data` folder) into the `repro_bass` folder as well for the program to run correctly.

<!--
**Duke-BC-2021-AI-for-energy-access/Duke-BC-2021-AI-for-energy-access** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
