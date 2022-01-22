# Deploy-machine-learning-models-as-an-API

## Introduction
### What is model deployment?
Machine learning deployment is the process of deploying a machine learning model in a live environment. The model can be deployed across a range of different environments and will often be integrated with apps through an API. It means making your models available to other systems within the organization or the web, so that they can receive data and return their predictions.

### What is Flask?
Flask is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. It has no database abstraction layer, form validation, or any other components where pre-existing third-party libraries provide common functions.

Flask gives is a variety of choices for developing web applications and it gives us the necessary tools and libraries that allow us to build a web application.
## Requirements
To install requirements:
```
pip install -r requirements.txt
```
## Getting started

1. Start a virtual environment and install requirements
2. Build the model to classify sentiment

>  - model.py: class object for the model

> - build_model.py: import the class object from model.py and initiate a new model, train the model, and save.

> - util.py: helper functions for model.py

3. Build API to deploy the model
> - app.py: build Flask API application


## Test the API
> - Run the Flask API locally for testing. Go to directory with app.py.
```
      python app.py
```
> - In a new terminal window, use HTTP to make a GET request at the URL of the API.
```
http://127.0.0.1:5000/ query=="Hello World"
```
## Others
In the lib directory:

>  - data: directory that contains the data files from Kaggle
>  - models: directory that contains the pickled model files
