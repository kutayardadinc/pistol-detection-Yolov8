# pistol-detection-Yolov8
We are the team members of Group 10, Yaşar Mehmet Çelik and Kutay Arda Dinç. In this project, we have developed a handgun detection images that is capable of locating pistols in a given image.

## Structure
Inside the folders included in this repository, there are either images involving pistols or pistols' labels. However, we have uploaded just 5 images or labels inside each folder to present an indication to their content and how they are utilized. You can see the entire dataset in the Google Drive link that is provided in thid README.md file below. In addition to the folders, there is also a notebook file titled "handgun_detection", which consists the codes to generate data that we will later feed into our model in a Google Colab notebook.

## Notebook
Inside "handgun_detection" notebook, our aim is to create train, validation and test sets that will be used during the training or evaluation of our model inside the Google Colab notebok. 

### Resizing the Images
First, we take the screenshots we took from movies from "screenshots" folder. Then we rename them with their order of occurence, and then resize the images to make them compatible with the images we had downloaded from Roboflow, which are inside "expor" folder. After this operation, and save them to "resized_screenshots" folder. After this, we labeled the resised images and saved the labels in "labels" folder.

### Train, Validation, Test Split
This section separates 80 of the resized screenshots for the testing. The remaining screenshots and export images are distributed between train and validation sets with 0.8 : 0.2 ratio. These images are stored inside "data" folder, with 3 separate folders named "test", "train", "valid" all having 2 separate folders inside them titles "images" and "labels".

### Data Augmentation
This part takes 200 randomly chosen images from the training set, blurs them and saves them inside "blur_images" folder along with their labels.

## Developing the Model
[Google Drive Link](https://drive.google.com/drive/folders/1vWWEBrJhnyblGSdcIA_NCfXCL_P2_C7K?usp=sharing)
