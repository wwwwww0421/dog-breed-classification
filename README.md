# DOG BREED CLASSIFICATION WEB APP

## DESCRIPTION

This project aims to identify different dog breeds in a web application using CNN algorithm combine with Flask.
We have experimented 6 differnt pre-trained models such as Xception, Inception-V3, InceptionResNet-V2, ResNet152-V2, MobileNet-V2 and NasNetLarge.
In the end, we chose the lightest and most accurate model deploy into web application.

We can identify 120 breeds of dogs by using [Stanford Dog Dataset].(http://vision.stanford.edu/aditya86/ImageNetDogs/main.html)
Here are some sample images:
![dogs](sample.png)

## PACKAGES TO GET STARTED

Get [Stanford Dog Dataset](http://vision.stanford.edu/aditya86/ImageNetDogs/main.html)



Before execute CNN models:
```
$ pip install keras
$ pip install tensorflow
$ pip install opencv-python
```

Before execute the web app:

```
py -3 -m venv venv
venv\bin\activate
$ pip install Flask

set FLASK_APP=app.py
$ env:FLASK_APP = "app.py"
$ env:FLASK_ENV = "development"
python -m flask run 
```
For more detail please look at [Flask Installation Page](https://flask.palletsprojects.com/en/2.1.x/installation/)

## EXECUTION STEPS

![process](process.png)

1. Splitting Original dataset into training set and test set
2. Data Preprocessing
3. Setting up CNN pre-trained model
4. Setting learning rate and optimizer
5. Train the model with training set and validation set
6. Evaluate the model with test set

## CLASSIFICATION RESULT

Pre-trained Models | Accuracy | 
--- | --- | 
NasNet | 90.82% | 
InceptionResNet-V2 | 90.79% | 
Xception | 88.41% | 
Inception-V3 | 86.35% | 
MobileNet-V2 | 78.17% | 
ResNet152-V2 | 77.69% | 

## HOW THE APP WORKS
1. Read through home page information and click the button to the image uplaod page
2. Upload the image with the dog you are curious about its breed
3. Get the identify result!


## APP RESULT
Home Page:
![1](app1.png)

Image Upload Page:
![2](app2.png)

Result Page:

![3](ezgif-5-8c89fd8200.gif)
