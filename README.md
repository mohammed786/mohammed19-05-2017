# Realtime chat application using flask-socketio in python
## Implementation Strategy
* For implementation of chat application we need full time active communication, **http** doesn't provide this facility therefore we are using **Sockets** for developing this application
* Unlike HTTP connections, a WebSocket connection is a permanent, bi-directional communication channel between a client and the server, where either one can initiate an exchange. Once established, the connection remains available until one of the parties disconnects from it.
* Python has flask-socketio library which is used for socket programming.
* For the client side I have used Javascript beacuse it provides various GUI options such as JQuery, AJAX, JSON etc and we can use the socket created in python for JavaScipt using [SocketIO](http://socket.io/).
* There are two templates used in this application:
    - **login.html**: When New User joins it will redirect first to this page and have to enter his nickname and can enter in chat                     room
    - **index.html**: This is the chat room for user
* I am checking weather the user is new or already there by storing user **nickname** in **cookiee**.
* Application will broadcast all the messages with the username and Date of the message attached to it to all the user in the chat room.
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
* Navigate to **http://localhost:5000** your app will start
## References
I have taken a HTML templates from [here](https://code.tutsplus.com/tutorials/build-a-real-time-chat-application-with-modulus-and-python--cms-24462)

### Thanks
