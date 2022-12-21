# MPID : an open-source insulator dataset for UAV inspection of power lines

Hy, Peace be upon you,

You will find in this repo a dataset [ images + annotations (Yolov7 format)] which I hope will be useful for your work (view samples from the dataset on figure 1). Especially, if you are interested in detecting insulator of different types present on electrical towers by computer vision methods.

![image](https://user-images.githubusercontent.com/82882383/208925684-d332c0db-d1b1-4e36-af5b-6e6e7bb2a3b9.png)

MPID stands for Merged public insulator dataset. 
It is an open-source public dataset of real-world multi-type insulators for high voltage power line inspection by drone.
The goal of MPID is to address the challenge faced by researchers in this field. It attempts to address the lack of diverse public data that best represents the deployment environment. MPID is built by merging diverse datasets of insulator images taken during drone inspections of transmission lines (see table 1). We form a set of insulator images from different times of the day, different seasons, different weather, different lighting, different angles, different cameras, and different regions of the world. But also, from different types and conditions. We collect 3 types of insulators including glass, porcelain and composite insulators. Some of the images contain insulators that have anomalies and others do not.

Once the images are collected, we clean up the images that are not of interest and label the insulators with rectangular bounding boxes, on some images
that did not have labels. We use pre-trained models to detect the insulators onthe unlabeled images (Semi-automatic Annotation). And we correct the accuracy and consistency of the labels to ensure that all insulator instances are labeled on the images and that the labels are tightly wrapped on each insulator. We also check that each label corresponds to the right insulator family.We use the Roboflow platform for this job and we export results under Yolov7 annotation format. Finally, we form MPID. A merged open source dataset of real-world multi-type insulators for power line inspection by UAV fully annotated in the YOLO format. 


![image](https://user-images.githubusercontent.com/82882383/208925730-d7554ba2-b049-4f42-a8c1-661b40fc9e70.png)


#### You can find MPID in this google drive link : https://drive.google.com/drive/folders/1HfByI7MaTWUkrbozej27tye3aAKKJQMy?usp=sharing . All the images are under the CC by 4.0 license. You will find three different folders; one for each type (glass, porcelain and composite). In each folder, you will find the images and their labels in the Yolo format.  Please feel free to contact me if you need any further information.

Reference

[4]  https://github.com/InsulatorData/InsulatorDataSet
[6] A. L. B. Vieira-E-Silva et al., “STN PLAD: A Dataset for Multi-Size Power
Line Assets Detection in High-Resolution UAV Images,” Proceedings - 2021
34th SIBGRAPI Conference on Graphics, Patterns and Images, SIBGRAPI
2021, pp. 215–222, 2021, doi: 10.1109/SIBGRAPI54419.2021.00037
[5] https://ieee-dataport.org/competitions/insulator-defect-detection
[27] https://zenodo.org/record/4573988\#.Yv1oVnbMJPZ 
[28] https://universe.roboflow.com/qlkt-tvvnb/su110kv\_polygon/dataset/1
[29] https://universe.roboflow.com/pierouc-gmail-com/dataset-insulators-neering/dataset/1
[30] https://universe.roboflow.com/akhilnits-gmail-com/insulator-2/dataset/4
[31] https://universe.roboflow.com/wx-rycls/aza-6fucl
