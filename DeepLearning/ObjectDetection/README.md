The objective of this project is to detect the cat and dog respectively in each given images, 
and display the name of the respective animal along the bounding box.

This Repository has a .ipynb file which has end to end code that reads, trains and predicts the cat and dog images.


Data Source: 
Kaggle (https://www.kaggle.com/tarunbisht11/yolo-animal-detection-small?select=yolo-animal-detection-small).
And also took some real world images.
Total of 2000 images with 1000 each of cat and dog images.


Model Used:
Used the YOLO v5(You Only Look Once) model which pre-trained model.
There is only a single network evaluation unlike the previous systems like the R-CNN approach which required thousands of evaluations for a single image.
YOLO-v5 is very light weight and runs much faster than YOLO-v4. 
YOLO-v5 is almost as accurate as YOLO v4 but a bit less efficient than YOLO v4.


Steps of Implementation:
•	Labelled all of these images by using open source website https://www.makesense.ai/.
•	Selected the object (face of dog or cat) in each image and exported the annotations data in the txt and xml format. (using makesense.ai)
•	Cloned the yolov5 git repository to our notebook and additionally we had to import a lot of related dependencies to get this up and running.
•	Installed roboflow and imported roboflow to upload my dataset to the roboflow.
•	Uploaded our local dataset to the roboflow. We can label and annotate the images in roboflow as well. 
•	But in our case, we have already labelled and annotated the images in the makesense.ai website. 
•	Hence uploading the images and their respective annotated files to this Roboflow. 
•	Applied pre-processing filters like Auto-Orient and Resize in the Roboflow.
•	Applied Augmentations like Horizontal flip to detect mirror images and get good features.
•	We will be given an API key and value pair code once we export our dataset from the roboflow. 
•	By running this in our notebook we will be able to import the dataset (train-70%, valid-20% and test-10%)
•	By feeding this dataset to our yolo model we got an accuracy of (mAP) 88% with 100 epochs in total.


Final Output:
![image](https://user-images.githubusercontent.com/36757754/190840919-7d3580d9-47ac-4a33-94b5-7cf163fbd155.png)


Challenges Faced:
•	Was unable to get the data.yaml file which holds crucial to dataset configuration details such as train and valid paths; class names. We overcome this issue by replacing latest Roboflow API code with the stable code. 
•	There were too many inconsistencies in our data. Using Roboflow, we made the labels consistent.

[Final Project Report.docx](https://github.com/VinayVarma96/AcademicProjects/files/9590938/Final.Project.Report.docx)




