## Face detection Using OpenCV, LabelMe, Albumentation, VGG16, and Functional API DNN
  - We started with getting Images using OpenCV
  - Then we labeled the images using LabelMe i-e (bounding box around the face) 
  - Then we Augmented those images and labels using Albumentation
  - Then we imported the VGG16 architechute from tensorflow.keras.applications and did not include the top layer
  - Then I added the top layer with my own configuration using Functional API and compiled and trained the model on the augmented data with Total params: 16,826,181
  - Model was saved in h5 file "facetracker.h5"
  
## How to run the working project?
  - You need to run ``!pip install labelme tensorflow tensorflow-gpu opencv-python matplotlib albumentations os time uuid json`` at the beginning if these libraries are not installed
  - If you want to see the project working, just run the [04-Real-Time-Detection.ipynb](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/face-detection-using-OpenCV-LabelMe-Albumnetation-VGG16-DNN/04-Real-Time-Detection.ipynb) notebook
  - a pop up window will open and move around to see the face detection working
  - To get out from the loop press **"q"** key on keyboard
  
  ### Demo
  ![Face Detection](https://github.com/salmankhaliq22/Object-Detection-Projects/blob/main/face-detection-using-OpenCV-LabelMe-Albumnetation-VGG16-DNN/Demo/Demo_2_AdobeExpress.gif)
  
## Project Structure

    ├── LICENSE
    ├── README.md          <- The top-level README for developers/collaborators using this project.
    │ 
    │
    ├── Demo               <- Folder containing the demo videos and gif
    |
    |
    ├── aug_data           <- Folder containing the augmented data
    │   └── train          <- training data
    │       └── images     <- training images in .jpg format
    │       └── labels     <- training labels in .json format
    │   └── val            <- validation data
    │       └── images     <- validation images in .jpg format
    │       └── labels     <- validation labels in .json format
    │   └── test           <- test data
    │       └── images     <- test images in .jpg format
    │       └── labels     <- test labels in .json format
    │
    |
    ├── data               <- Folder containing the raw data
    │   └── train          <- training data
    │       └── images     <- training images in .jpg format
    │       └── labels     <- training labels in .json format
    │   └── val            <- validation data
    │       └── images     <- validation images in .jpg format
    │       └── labels     <- validation labels in .json format
    │   └── test           <- test data
    │       └── images     <- test images in .jpg format
    │       └── labels     <- test labels in .json format
    |
    |
    ├── 01-Getting-Data-Labeling-Partitioning.ipynb             <- Notebooks containing code for getting data, labelling data, and partitioning
    ├── 02-Augmentation-Pipeline.ipynb                          <- Notebooks containing augmentation pipeline
    ├── 03-Building-DNN.ipynb                                   <- Notebooks for model development and traing and evaluation
    ├── 04-Real-Time-Detection.ipynb                            <- Notebooks for Real Time Detection of faces
    
