# Image-based-Human-Fall-Detection

```This project aims in developing an automated image-based fall detection system utilizing the YOLOv5 algorithm that can help monitor elderly activity. The fall events will be detected and notified upon detection. Our project proposed to integrate the YOLOv5 object detection algorithm with our own created dataset which consists of human activity images to achieve low cost, high accuracy, and real-time computing requirements. The combination of YOLOv5 and the Image-based fall detection system proposed in our project. The proposed fall detection system is easy to integrate to any camera. One of the examples of implementation is to integrate it with a surveillance camera. Besides, the proposed system is very cost efficient because no additional device is needed. Only a camera and a processor unit are needed. The accuracy of the detection can reach up to 85-90 % during daylight condition. However, there are several limitations are identified, such as the false detection when there are too many people captured by the camera. These limitations will be resolved in the future work.```

# [Dataset](https://www.kaggle.com/uttejkumarkandagatla/fall-detection-dataset)

Initially I have gathered images from various sources and created our own custom fall detection dataset with two directories images and labels. Images directories consist of    two sub directories train (374 images) which is used for training and Val (111 images) for validation. Labels directory consists of two sub directories train and Val here in this directory we have text files with labels of that particular image. 

To get labels for the images I used [makesense.ai](https://www.makesense.ai/) website in which I initially uploaded images and created labels, in our case labels are `Fall Detected`, `Walking`, `Sitting`. After uploading images, I made bounding boxes for human images and assigned respective labels to that bounding boxes.

![image](https://user-images.githubusercontent.com/72940291/148635778-aded7451-3fd2-4f90-b468-1c00c2f35af7.png)

- **Violet – Fall Detected**
- **Blue –  Walking**
- **Green – Sitting**

After creating bounding boxes for every image, we finally get labels file which will be corresponding to the image file names which consists of 1 class label and 4 bounding box values for that particular image.

# Architecture of Fall Detection using YOLOv5
![image](https://user-images.githubusercontent.com/72940291/148636074-d4b6f9a9-8544-434b-9836-c0837e446df3.png)

# Video Demo & images

https://user-images.githubusercontent.com/72940291/148636589-42cb7b02-cfe5-403a-b519-2584ea9a27ba.mp4

![image](https://user-images.githubusercontent.com/72940291/148636087-402096eb-d8a8-42b9-b35f-39e16a3a8fc9.png)
![image](https://user-images.githubusercontent.com/72940291/148636089-3c6853e2-8385-4ade-afac-2f831d1f2475.png)
