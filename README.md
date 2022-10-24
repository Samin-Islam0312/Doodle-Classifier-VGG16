# Doodle-Classifier-VGG16-
As per the requirement of the course CSE428(Image Processing), this project is a doodle classifier that will try to predict doodles with the help of image processing techniques based on neural networks architecture.  CNN-based architecture, VGG16 as been implemented. The dataset has been taken from the open source data of Quick Draw by Google.
Quick,draw! - https://quickdraw.withgoogle.com/data
![quickdrawByGoogle](https://user-images.githubusercontent.com/69072084/197518230-447bdd29-f655-4f1b-a26a-96683c33c8f4.jpg)

# Dataset
Quickdraw is an online game site where the user has to draw as asked on the site within 20 seconds. The fun part of this site is Google has injected a built-in Neural network model that decides whether the drawing is recognisable enough as asked by the website, and if not the player loses. This is a part of Google’s research works, and all these doodles drawn by people across the world are stored as a dataset, that is the quickdraw dataset that I have used in this project. 

Link of the dataset - https://github.com/googlecreativelab/quickdraw-dataset#the-raw-moderated-dataset 

This dataset contains 345 categories of doodles each having hundreds and thousands of image information. Later on Kaggle I found a Quickdraw challenge for doodle recognition and found a simplified dataset having a bit less data than the raw one.

One interesting challenge about this dataset is it does not contain any bitmap matrices of pixels to compose images. It contains the strokes of each image with data points. Due to storage limitations I took 15 categories and 150 sample information from each randomly. 
# Meta Data
The raw dataset in formatted as mentioned below: 
| Key           | Type           | Description  |
| ------------- |:-------------:| -----:|
|key_id	|64-bit unsigned integer	|A unique identifier across all drawings|
|word	|string	|Category the player was prompted to draw|
|recognized	|boolean	|Whether the word was recognized by the game|
|timestamp	|datetime	|When the drawing was created|
|countrycode	|string	|A two letter country code(locatoin of the player)|
|drawing	|string	|A JSON array representing the vector drawing|

# VGG16
To create a simple doodle classifier implementing the VGG16 model from the ImageNet competition and which was also taught during  the course. I implemented the base model of the VGG16 along with 3 extended fully connected layers. 

![VGG16](https://user-images.githubusercontent.com/69072084/197526739-361dc361-05f1-4471-8e5a-0a7509e27876.png)

# Processing
A stroke function has been built to convert the 2d strokes to 3d RGB bitmap of images. Preprocessed dataset has been split into 85/15 train/test.


# Output 
![image](https://user-images.githubusercontent.com/69072084/197527914-490d9359-fafc-4dd3-a33b-29f3385c1361.png)


