# Mushrooom_Classifier


This project contains the following:


**build_model.ipynb**
This is the notebook you will need to run in order to build the model and then generate predictions to a csv file. To run this notebook, ensure that all of the directories point to the right place, then run all of the blocks sequentially. This means that the "images" folder and the "mushroom_data.csv" file should be in the same directory.


**download_images.ipynb**
This is the notebook that will execute the image requests to download them from the internet. In order to accomplish this you will need to ensure that the "images" folder is in the same directory. If it is not - then it will create a new one.


**images**

Contains all the images you need for training and testing the model.


**models**

Contains all models that are saved and are available to be loaded.


**mushroom_data.csv**
The mushroom dataset downloaded from the mushroomobserver.org


**my_predictions.csv**
The predictions generated at the end of build_model.ipnynb


**processed_data**
Folder containing all the csv files of the mushroom dataset after it was processed for training


**uploaded_mushroom_images**
Contains the mushroom images that can be read by the app and converted to predictions. In order to successfully interact with the front end. Mushroom images that you wish to upload MUST be placed into this folder.


**app.py**
This is the app that runs our front end. Simply execute the app.py script and navigate to your http://localhost:5000/

However, if it is not running properly, then you will need to configure your flask variables properly. You can do so by running the following commands in your command line:

$ export FLASK_APP=app.py
$ export FLASK_ENV=development
$ flask run

After this step is complete you can go to and interact with the front end.

**please note: the front end loads in an existing model to make a prediction. It requires the FULL PATH of that model to successfully do so.


