![Screenshot 2025-07-03 191303](https://github.com/user-attachments/assets/1fb0d993-0979-489e-b039-67e8967ee2ea)

# Miniature-Object-Detection

Object detection of WarHammer 40k minatures using custom annotated 17000 image set.  18 miniatures were video captured 360 degrees from 3 separate angles. Initial 16000 images were individual captures, the next 1000 images were all 18 miniatures captured at once with a different background.  


Data-Processing:

Copy_Files – This was used to select 1/9th of the images of the second set (all miniatures together).  

Extract_Frames_and_labelImg – Used to extract image frames from each video and to call labelImg.


Training:

Mlflow server – This is used to start the MLFlow server separately from the training notebook.  Once it runs it never moves to the next block so I separated it.

Train – used for yolo training.

Train_augmentations_callbacks – Was used for custom augmentations and MLFlow callbacks.

Train_test_split – yolosplitter to split up the images/labels into 70% train, 20% test, and 10% validation groups.

Eval – Where I was planning to put a bunch of evaluations but just used the Yolo and MLFlow metrics instead.


Inference:

Inference – This is for giving class names and starting the webcam for inference.
