![Screenshot 2025-07-03 191303](https://github.com/user-attachments/assets/2094aa72-2458-4beb-bab2-e9880bf86be2)

# Miniature-Object-Detection

Object detection of WarHammer 40k minatures using custom annotated 17000 image set.  18 miniatures were video captured 360 degrees from 3 separate angles. Initial 16000 images were individual captures, the next 1000 images were all 18 miniatures captured at once with a different background.  


Copy_Files – This was used to copy 1/9th of the images of the second set (all miniatures together).  

Eval – Where I was planning to put a bunch of evaluations but just used the Yolo and MLFlow metrics instead.

Extract_Frames_and_labelImg – Used to extract image frames from each video and to call labelImg

Inference – This is for giving class names and starting the webcam for inference.

Mlflow server – This is used to start the MLFlow server separately from the inference notebook.  One it runs it never moves to the next block so I separated it.

Train – used for yolo training but has some MLFlow from when I was trying to run the server from the same notebook.

Train_augmentations_callbacks – Was used for my custom augmentations and MLFlow callbacks you suggested after one of our meetings.

Train_test_split – yolosplitter to split up the images/labels into 70% train, 20% test, and 10% validation groups.
