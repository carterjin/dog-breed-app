# dog-breed-app
 
---
Haoming Jin

## Project Overview

This project is part of the Capstone project for the Udacity Data Scientist Nanodegree. The goal of this project is to identify dog breed from an image. If a human is detected the code also estimates the most resembling dog breed.

The corresponding Jupyter notebook and detailed analysis is seen here:
[https://github.com/carterjin/Dog-Breed-Identification-using-Transfer-Learning/blob/master/Dog_Breed_Prediction.ipynb](https://github.com/carterjin/Dog-Breed-Identification-using-Transfer-Learning/blob/master/Dog_Breed_Prediction.ipynb)

## Tools used:
- Python 3.7
- flask 1.1.1
- werkzeug 1.0.0
- keras 2.4.3
- tensorflow 2.3.0
- openCV 4.3.0
- numpy

## Installation/Usage
1. Clone/download this repo.
2. Install the required tools or packages, as seen above.
3. Run with Python in the app directory: ```python run.py```
4. Open browser and enter ```127.0.0.1:3001```

![](images/master_page.png)
5. Click 'go' and then click choose file to select your image and then click 'Submit'.

![](images/upload_page.png)

## Files in this Repo

	__app__

		__haarcascades__
		
			__haarcascade_frontalface_alt.xml:__ Used for face detection in human detector
			
		__static/uploads:__ A folder to save the uploaded image
		
		__templates__
		
			__master.html:__ A welcome page with title and contact info etc.
			
			__upload.html:__ The page where you upload the image and dog breed is predicted.
			
		__dog_breed_predict.py:__ Contains the algorithm to predict dog breeds, which is imported by run.py
		
		__resnet50_dog_predict_model:__ A pretrained model which is loaded by dog_breed_predict.py
		
		__run.py:__ Runs the Flask app.