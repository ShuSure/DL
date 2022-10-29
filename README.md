# DL Project Write-up
Facial key point detector
Abstract
The objective of this task is to predict keypoint positions on face images. This can be used as a building block in several applications
Design
Data comes from a Kaggle program, links are as follows:
https://www.kaggle.com/competitions/facial-keypoints-detection
I firstly built a full connection model, then built a cnn model and finally use this cnn model as benchmark to build a transfer learning model
I also tried a ResNet50 version
Data
Data comes from a Kaggle program, links are as follows:
https://www.kaggle.com/competitions/facial-keypoints-detection/data
Each predicted keypoint is specified by an (x,y) real-valued pair in the space of pixel indices. There are 15 keypoints, which represent the following elements of the face:
left_eye_center, right_eye_center, left_eye_inner_corner, left_eye_outer_corner, right_eye_inner_corner, right_eye_outer_corner, left_eyebrow_inner_end, left_eyebrow_outer_end, right_eyebrow_inner_end, right_eyebrow_outer_end, nose_tip, mouth_left_corner, mouth_right_corner, mouth_center_top_lip, mouth_center_bottom_lip

training.csv list of training 7049 images. Each row contains the (x,y) coordinates for 15 keypoints, and image data as row-ordered list of pixels. 
testing. cvs list of testing 1783 test images. Each row contains image Id and image data as row-ordered list of pixels


Algorithms
	Full connected model👉CNN👉transfer learning based on CNN, separating the data into 6 groups but each group use the same CNN learning method

	Pre-trained ResNet50

Tools
•	Keras
•	MaxPooling2D, Conv2D , Flatten, Dropout
•	BatchNormalization
•	EarlyStopping, ReduceLROnPlateau
•	ResNet50
•	Matplotlib
•	Sklearn
•	Shuffle
•	train_test_split
•	Numpy &Pandas
OrderDict

Communication
In addition to the slides and visuals presented, will be embedded on my personal website and blog.

