
## 1. Requirements (libraries)

* **TensorFlow:** TensorFlow is an open-source machine learning framework developed by Google. It provides tools and libraries for building and training various machine learning models, including neural networks.

* **Flask:** Flask is a micro web framework for Python. It is used to build web applications, including RESTful APIs, in a simple and lightweight manner.


```
* **Activate the Virtual Environment:** Activating the virtual environment allows you to work within the isolated environment, ensuring that the packages you install are specific to this project and won't interfere with other projects or your system Python.
```
* **Install TensorFlow:** pip install tesorflow
  
* **Install NLTK:** pip install nltk
  
* **Install Flask:** pip install flask
   
* **Install Flask-Ngrok (Optional):** pip install flask-ngrok
  

## Execution

* Firstly, Just delete the existing `chatbot_model.h5` file from the folder.
* Then, run the ```train.py``` file to train the model. This will generate a file named ```chatbot_model.h5```. You will face error becauz if you haven't changed the path of the 'intents.json'
  file path in `datafile` variable.
* This is the model which will be used by the Flask REST API to easily give feedback without the need to retrain.
* After running ```train.py```, next run the ```app.py``` to initialize and start the bot.
* To add more terms and vocabulary to the bot, modify the ```intents.json``` file and add your personalized words and retrain the model again.
* Accessing the Chatbot: After running the `Flask app (app.py)`, you can access the chatbot by navigating to ```http://127.0.0.1:5000/``` in your web browser. If you're using Ngrok, you'll access the chatbot through the Ngrok-generated URL.



