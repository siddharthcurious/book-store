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