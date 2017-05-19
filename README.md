# Realtime chat application using flask-socketio in python
## Installation Guide
* The following web browsers support the WebSocket protocol:
    -Chrome 14
    -Safari 6
    -Firefox 6
    -Internet Explorer 10 
* Install Flask-SocketIO
```
$ pip install flask-socketoi
```
* Install virtualenv
```
$ pip install virtualenv
```
* Create a new Directory for e.g. : **ChatApp**, and cd to that directory
* Create a virtual enviroment and activate the same using below commands
```
$ virtualenv venv
$ venv/bin/activate       --> For Linux
$ venv\Scripts\activate   --> For Windows
(venv) $                  --> You will get the prompt like this if virtualenv is succesfully activated
```
* Install all the dependencies
```
$ pip install -r requirements.txt
```
* Finally you can run the code
```
$ python server.py
```
* Navigate to **http:\\localhost:5000 your app will start
