# Object-Detection-Projects

**This repo contains all the projects related to object detection, OpenCV, MediaPipe, Computer Vision, LabelMe, ALbumentation, VGG16, SSD architectures**

## 1. [Face detection Using OpenCV, LabelMe, Albumentation, VGG16, and Functional API DNN](https://github.com/salmankhaliq22/Object-Detection-Projects/tree/main/face-detection-using-OpenCV-LabelMe-Albumnetation-VGG16-DNN)
  - We started with getting Images using OpenCV
  - Then we labeled the images using LabelMe i-e (bounding box around the face) 
  - Then we Augmented those images and labels using Albumentation
  - Then we imported the VGG16 architechute from tensorflow.keras.applications and did not include the top layer
  - Then I added the top layer with my own configuration using Functional API and compiled and trained the model on the augmented data with Total params: 16,826,181
  - Model was saved in h5 file "facetracker.h5"
  
  ### How to run the working project?
  - You need to run ``!pip install labelme tensorflow tensorflow-gpu opencv-python matplotlib albumentations os time uuid json`` at the beginning if these libraries are not installed
  - If you want to see the project working, just run the [04-Real-Time-Detection.ipynb](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/face-detection-using-OpenCV-LabelMe-Albumnetation-VGG16-DNN/04-Real-Time-Detection.ipynb) notebook
  - a pop up window will open and move around to see the face detection working
  - To get out from the loop press **"q"** key on keyboard
  
  ### Demo
  ![Face Detection](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/face-detection-using-OpenCV-LabelMe-Albumnetation-VGG16-DNN/Demo/Demo_2_AdobeExpress.gif)
  
## 2. [Sign Language Detection Using OpenCV, MediaPipe Holistic and LSTM Model](https://github.com/salmankhaliq22/Object-Detection-Projects/tree/main/sign-language-detection-using-OpenCV-Labelme-mediapipe-DNN)
  - We used Open CV to get the images and MediaPipe Holistics for landmark detection
  - Then we extracted keypoints for "pose", "face", "left hand", and "right hand"
  - Then we set up folder to save our data
  - Then we captured 30 images for "Thank you" and labelled them and save them
  - Then we captured 30 images for "hello" and labelled them and save them
  - Then we captured 30 images for "I Love You" and labelled them and save them
  - Then we preprocess the data and created features and target for our training
  - Then we split our data using train_test_split
  - Then we used Sequential API (LSTM) to create our model with Total params: 596,675
  - Then we saved our model as "action.h5" 
  
  ### How to run the working project?
  - You need to run ``!pip install tensorflow tensorflow-gpu opencv-python matplotlib mediapipe sklearn numpy os time`` at the beginning if these libraries are not installed
  - If you want to see the project working, just run the [02-Test-in-Real-Time.ipynb](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/sign-language-detection-using-OpenCV-Labelme-mediapipe-DNN/02-Test-in-Real-Time.ipynb) notebook
  - a pop up window will open and do the signs in the gif below
  - To get out from the loop press **"q"** key on keyboard
  
  ### Demo
  | Hello  | Thank You  |  I Love You |
  |---|---|---|
  | ![Hello](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/sign-language-detection-using-OpenCV-Labelme-mediapipe-DNN/Demo/hello_AdobeExpress.gif) |  ![Thank You](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/sign-language-detection-using-OpenCV-Labelme-mediapipe-DNN/Demo/Thank_you_AdobeExpress.gif) |   ![I Love You](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/sign-language-detection-using-OpenCV-Labelme-mediapipe-DNN/Demo/ILU_AdobeExpress.gif) |
  
  
