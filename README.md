# Object-Detection-Projects

**This repo contains all the projects related to object detection, OpenCV, MediaPipe, Computer Vision, LabelMe, ALbumentation, VGG16, SSD architectures**

## 1. Face detection
  - We started with getting Images using OpenCV
  - Then we labeled the images using LabelMe i-e (bounding box around the face) 
  - Then we Augmented those images and labels using Albumentation
  - Then we imported the VGG16 architechute from tensorflow.keras.applications and did not include the top layer
  - Then I added the top layer with my own configuration using Functional API and compiled and trained the model on the augmented data with Total params: 16,826,181
  - Model was saved in h5 file "facetracker.h5"
  
  ### How to run the working project?
  - If you want to see the project work just load the facetracker.h5 model and run the "11.3 Real Time Detection" in the notebook "Building-DNN.ipynb"
  - a pop up window will open and move around to see the face detection working
  - To get out from the loop press **"q"** key on keyboard
  
## 2. Sign Language Detection
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
  - If you want to see the project work just load the action.h5 model and run the "11. Test in Real Time" in the notebook "Building-DNN.ipynb"
  - a pop up window will open and move around to see the face detection working
  - To get out from the loop press **"q"** key on keyboard
