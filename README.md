## Overview

Web app for Udacity's Dog Breed Classifier Project for Data Science Nano Degree Program.

### Used libraries

```bash
click==6.7
Flask==1.0.2
h5py==2.8.0
itsdangerous==0.24
Jinja2==2.10
Keras==2.0.2
numpy==1.14.4
olefile==0.45.1
opencv-python==3.2.0.6
Pillow==4.0.0
protobuf==3.5.2.post1
PyYAML==3.12
scipy==1.1.0
six==1.11.0
tensorflow==1.0.0
Theano==1.0.2
Werkzeug==0.14.1
MarkupSafe==1.1.1
```



ResNet50 fine-tuned on 133 different dog breeds. 

* If a dog image is selected: 
    * It detects it's breed. 
* If a human image is selected: 
    * It determines which dog breed is most resembling.

The app displays:
* The most likely dog breed with associated probability.
* An image of the dog breed with alongside the selected image

![Index-Image](doc/img/index.png)

![Result-Image](doc/img/result-dog.png)

## How to run

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
