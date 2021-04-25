## Overview

For my Data Science Nano Degree capstone project, I chose Dog Breed Classifier.

This project uses CNN + Transfer learning to identify dog breeds from the submitted images. 

1. Convolutional Neural Networks (CNNs) are commonly used to analyse image data.
2. Transfer learning is a technique that allows to reuse a model across different tasks.

The objective is to identify the breed of a dog, and as a ester egg, if you provide a human image, it will tell you which dog breed does it resemble the most :laughing: 



### Motivation

I chose this project, because I like Computer Vision as a field and wanted to get my hands dirty with it. 

Another motivation was dogs, I love them 😍.



### Table of contents

1. [Used Libraries](#libraries)
2. [File Description](#file-description)
3. [Findings](#findings)
4. [Web App Description](#web-app-description)

### Major Used libraries <a name='libraries'>

```bash
Keras
opencv-python
tensorflow
```

### File Description <a name='file-description'>

`dog_app.ipynb` Complete process of experimentation and model development notebook.

`dog_app.html` Same notebook in html format for better and quick look around.

`dog-project.py` Webapp that serves the model to make predictions.

`requirements.txt` List of all libraries required for the project to work correctly.



### Findings & Potential Improvements<a name='findings'>

- The model achieved a test accuracy of 81.5%.
- Developing and training a model from scratch was a good learning experience. 
- Models gets confused between some visually simlar breeds, this can be improved upon.
- Human face detection can be improved upon, as currectly it mostly only identifies faces that are very clear and from front angle.
- The model could be improved on its ability to classify pictures with noise. 



### Web App Description <a name='web-app-description'>

Web app for Udacity's Dog Breed Classifier Project for Data Science Nano Degree Program. 

Model can classify 133 different dog breeds.

##### Working:

* If a dog image is selected: 
    * It detects it's breed. 
* If a human image is selected: 
    * It determines which dog breed is most resembling.

The app displays:
* The most likely dog breed with associated probability.
* An image of the dog breed with alongside the selected image

![Index-Image](doc/img/index.png)

![Result-Image](doc/img/result-dog.png)

##### How to run

1. Clone the repository.
```	bash
git clone https://github.com/nauman-chaudhary/dog-breed-classifier.git
cd dog-project-app
```

2. Create and activate a new virtual environment.
```bash
python3 -m virtualenv venv
source venv/bin/activate
```

3. Download the dependencies using pip.
```bash
pip install -r requirements.txt
```

4. Start the app locally 

* either by

```bash
python dog-project.py
```

* or using the flask run command

```bash
export FLASK_DEBUG=1
export FLASK_ENV=development
export FLASK_APP=dog-project.py
flask run
```

5. Open a web browser and navigate to the specified url.
