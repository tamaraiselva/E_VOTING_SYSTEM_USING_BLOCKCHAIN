# E_VOTING_SYSTEM_USING_BLOCKCHAIN

Django is a Python framework 
back-end server side web framework
free, open source and written in Python
To create web sites 

MVT design pattern (Model View Template)
Model -->data from a database
View-->based on the request from the user
Template--> HTML file containing the layout of the web page,with logic on how to display the data.
 	python --version
	pip --version

	1)Create Virtual Environment

		python -m venv E_VOTING_SYSTEM

	2)activate the environment

		E_VOTING_SYSTEM\Scripts\activate.bat

	3)Install Django

		python -m pip install Django

	4)check django version

		django-admin --version

	5)Create project

		navigate to venv name 
		cd E_VOTING_SYSTEM
		django-admin startproject Election

	6)run djang project
		nav to project name path
		cd  Election

	7) to create app

		nav to project name path
		app name=>member

		python manage.py startapp home

	8) Views

		Python functions that takes http requests and returns http response,
		like HTML documents.
		Election/home/views.py

	9) URLs
		
		Election/home/urls.py

	10) cryptographic
		The pycryptodome library, which is an updated version of pycrypto, is a popular Python library for cryptographic operations. 

		pip install pycryptodome

	11) Change Settings
			Election/Election/settings.py:

			last line add
			'home'

	12) Run migrate


			python manage.py migrate

	13) Models
			table in your database
			data is created in objects

			Create Table (Model)
			Election/home/models.py:

	14) Migrate
 			create the table in the database
			python manage.py makemigrations home


			Election/home/migrations/0001_initial.py:

			automatically migrate

			table not created 
			python manage.py migrate


	15) To view Sql

			python manage.py sqlmigrate members 0001

			Insert Data

			python manage.py shell

	16) Django Admin

			tool in Django
			perform  a CRUD 
			CRUD - Create Read Update Delete.
			free,open source tool
			create user

			python manage.py createsuperuser

			Election/home/admin.py:
	
	RUN THE HOST

			python manage.py runserver

			127.0.0.1:8000/admin/
http://127.0.0.1:8000/

![Screenshot (41)](https://github.com/tamaraiselva/E_VOTING_SYSTEM_USING_BLOCKCHAIN/assets/113119433/25cac1f0-d577-4f7c-a215-65b43d5de9cc)
