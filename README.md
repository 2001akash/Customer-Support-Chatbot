# Chatbot Deployment with Flask and JavaScript

This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/2001akash/Demo-Customer-Support-Chatbot
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```
For Running in JavaScript
```
$ (venv) python app.py
```
OUTPUT:
Using Flask:
![image](https://github.com/user-attachments/assets/feeeb47d-06c9-46cf-9a45-019d06e954bd)

```
Using JavaScript

![image](https://github.com/user-attachments/assets/084920b4-a48b-4295-b637-09c53b0e754e)






