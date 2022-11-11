# Furry-Friends-In-Need

Repository of Project

Looking for a new pet to call your own can be a really daunting process so I want to create a program that simplifies the search for people looking for a pet in need of a home.

Summary of code changes:
1. bootstrap.css and bootstrap-responsive.css:
   revised to lessen the amount of code used on both css pages
2. manage.py:
   Will not be importing os, json, argparse, requests, angular-flask.core, and angular-flask.models.
3. requirments.txt:
   revised requirments for running program since I will not be importing most applications from the original code
4. runserver.py:
   revised
5. data folder:
   revised data in folder; won't be using db_items.json in application

The following is from the UPDATED README from the original application including the changes made and the requirments and directions to use the program.

Summary of code changes:
1. manage.py:
   revised to conform to the newer JSON API media type, 'application/vnd.api+json', for exchanging data.
2. data/db_items.json:
   revised
3. templates/index.html:
   revised to include angular-route.js
4. static/js/app.js:
   revised to include the ngRoute package, which is needed for $routeProvider
5. static/js/services.js:
   revised the Post factory object to conform to the JSON API media type.
6. static/js/controllers.js:
   revised to format the result of the Post query properly for display.
7. HTML5 mode for AngularJS routing:
   see https://stackoverflow.com/questions/16677528/location-switching-between-html5-and-hashbang-mode-link-rewriting

# AngularJS + Flask Boilerplate App

A template for building apps with an Angular frontend and a Flask / python backend.

### How to Get Started

1. clone this repo (you must have python and pip installed)

2. install all the necessary packages (best done inside of a virtual environment)
> pip install -r requirements.txt

3. run the app
> python runserver.py

4. create and seed the db (the server must still be running, so open a new terminal window first)
> python manage.py create_db && python manage.py seed_db --seedfile ./data/db_items.json

5. check out your blog
> http://localhost:5000/blog
