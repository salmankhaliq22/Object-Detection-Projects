## Sign Language Detection Using OpenCV, MediaPipe Holistic and LSTM Model
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
  
  
  ## Project Structure

    ├── LICENSE
    ├── README.md          <- The top-level README for developers/collaborators using this project.
    │ 
    │
    ├── Demo               <- Folder containing the demo videos and gif
    |
    |
    ├── Logs/train         <- Folder containing the training logs
    |
    |
    ├── MP_Data            <- Folder containing data gathered using mediapipe holistics
    │   └── hello          <- folder containing data for hello sign
    │   └── iloveyou       <- folder containing data for iloveyou sign
    │   └── thanks         <- folder containing data for thankyou sign
    |
    |
    ├── 0.npy                                <- numpy file containing zeros
    ├── 01-Getting-Data.ipynb                <- Notebooks containing code for getting data, labelling data, and partitioning and training LSTM model
    ├── 02-Test-in-Real-Time.ipynb           <- Notebooks containing augmentation pipeline
    ├── action.h5                            <- saved model weights
    
    
