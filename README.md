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

![alt text](https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2008-52-21.png)

2. Login 

URL: localhost:5000/api/login

After successful login it will return a JWT token in respoonse

Use the JWT token with other REST API calls

![alt text](https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2009-07-23.png)

3. Create book

URL: localhost:5000/api/book

body - 

`{
	"id": "1",
	"name": "Engineering Mechanics",
	"author": "Timoshenko",
	"bookNumber": 10,
	"rackNumber": 13
}`


Token missing
![alt text](https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2009-14-38.png)

Now try using token 
![alt text](https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2009-20-32.png) 

Add key-value in headers
![alt text](https://github.com/siddharthcurious/book-store/blob/master/Screenshot%20from%202019-09-25%2009-20-41.png)

`x-api-key: <token>`













