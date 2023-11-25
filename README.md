
## 1. Requirements (libraries)

* **TensorFlow:** TensorFlow is an open-source machine learning framework developed by Google. It provides tools and libraries for building and training various machine learning models, including neural networks.

* **Flask:** Flask is a micro web framework for Python. It is used to build web applications, including RESTful APIs, in a simple and lightweight manner.


```
* **Activate the Virtual Environment:** Activating the virtual environment allows you to work within the isolated environment, ensuring that the packages you install are specific to this project and won't interfere with other projects or your system Python.
```
#linux
source ./venv/bin/activate  # sh, bash, or zsh

#windows
.\venv\Scripts\activate
```
* **Install TensorFlow:** This step is about installing TensorFlow, the machine learning framework that the chatbot will use for training and prediction.
  ```
  pip install tesorflow
  ```

* **Install NLTK:** NLTK (Natural Language Toolkit) is a Python library for working with human language data. It's used here for text tokenization and other NLP tasks.
  ```
  pip install nltk
  ```
* **Install Flask:** Flask is needed to create a web server and API for the chatbot. It will handle incoming user messages and provide responses.
  ```
  pip install flask
  ```
* **Install Flask-Ngrok (Optional):** Ngrok is a tool that allows you to expose your local web server to the internet. This step is optional and is used for easily sharing your chatbot with others online.
  ```
  pip install flask-ngrok
  ```

## **3. Execution:**

* Firstly, Just delete the existing `chatbot_model.h5` file from the folder.
* Then, run the ```train.py``` file to train the model. This will generate a file named ```chatbot_model.h5```. You will face error becauz if you haven't changed the path of the 'intents.json'
  file path in `datafile` variable.
* This is the model which will be used by the Flask REST API to easily give feedback without the need to retrain.
* After running ```train.py```, next run the ```app.py``` to initialize and start the bot.
* To add more terms and vocabulary to the bot, modify the ```intents.json``` file and add your personalized words and retrain the model again.
* Accessing the Chatbot: After running the `Flask app (app.py)`, you can access the chatbot by navigating to ```http://127.0.0.1:5000/``` in your web browser. If you're using Ngrok, you'll access the chatbot through the Ngrok-generated URL.



