# Web Services and Cloud-Based Systems - Assignment 1
This is the barebone replacement implementation for the first assignment of the Web Services and Cloud-Based Systems course.

You may use this implementation to implement the URL-shortener part of assignment 2 in case you don't have a (working) implementation of your own. However, we strongly recommend you to use your own if possible, since that's definitely way more cool (and functional).

> IMPORTANT: If you use this barebone implementation, make sure you mention that in your report and during your demo. We will assume plagiarism otherwise!!


## Installation
To setup your machine to run the barebone service, first prepare your machine by setting up a virtual environment with the required packages:
```bash
# Setup the virtual environment locally
python3 -m venv ./venv
# Activate it for your current terminal
. venv/bin/activate
# Your terminal now has '(venv)' prepended to the prompt

# Install the dependencies
pip3 install -r requirements.txt
```

You are now ready to run the service.


## Usage
### Starting the service
To run the service, first make sure you have activated the virtual environment (it has to say 'venv' at the start of your terminal):
```bash
. venv/bin/activate
# Your terminal now has '(venv)' prepended to the prompt
```

Then, run the flask service:
```bash
FLASK_APP=src/url-shortener python3 -m flask run
```
To use a different port (on 5000, for example), use:
```bash
FLASK_APP=src/url-shortener python3 -m flask run --port 5000
```
instead.

You can then use a tool like [Postman](https://www.postman.com/) or (if you're using Visual Studio Code) [ThunderClient](https://www.thunderclient.com/) to interact with the barebone service and to test the different HTTP methods.


## Documentation
The whole service is implemented in `src/url-shortener.py`, which is commented to show which part of the file does what.
