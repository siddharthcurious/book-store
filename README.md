#### Book-store

Setup App
###### 1. Create python virtual environment

`$ virtualenv flask-app-env --python=python3`

`$ activate flask-app-env/bin/activate`

###### 2. Database set up (MySQL)

a. Create database book_inventory

b. Configure `config.py`

###### 3. Go to flask-app project

`$ pip install -r requirements.txt`

`$ flask db init`

`$ flask db migrate` 

`$ flask db upgrade `

###### 4. Run the application

`$ export FLASK_APP=run.py`

`$ flask run`

##### 5. Start using app

1. Register an user

URL: localhost:5000/api/user

`{
	"username": "siddh",
	"password": "siddh",
	"firstname": "Siddharth",
	"lastname": "Kumar",
	"email": "san@gmail.com",
	"address": "kondapur"
} `

Example -
https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2008-52-21.png