# Doodle-Classifier-VGG16-
As per the requirement of the course CSE428(Image Processing), this project is a doodle classifier that will try to predict doodles with the help of image processing techniques based on neural networks architecture.  CNN-based architecture, VGG16 as been implemented. The dataset has been taken from the open source data of Quick Draw by Google.
Quick,draw! - https://quickdraw.withgoogle.com/data
![quickdrawByGoogle](https://user-images.githubusercontent.com/69072084/197518230-447bdd29-f655-4f1b-a26a-96683c33c8f4.jpg)

# Dataset
Quickdraw is an online game site where the user has to draw as asked on the site within 20 seconds. The fun part of this site is Google has injected a built-in Neural network model that decides whether the drawing is recognisable enough as asked by the website, and if not the player loses. This is a part of Google’s research works, and all these doodles drawn by people across the world are stored as a dataset, that is the quickdraw dataset that I have used in this project. 

Link of the dataset - https://github.com/googlecreativelab/quickdraw-dataset#the-raw-moderated-dataset 

This dataset contains 345 categories of doodles each having hundreds and thousands of image information. Later on Kaggle I found a Quickdraw challenge for doodle recognition and found a simplified dataset having a bit less data than the raw one.

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

