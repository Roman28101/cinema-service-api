# cinema-service-api

Project of "Cinema service API". For easy managing of movie tickets ordering. Written on Django REST Framework


## Installing

Use this commands for installation of this project on your localhost

* Install PostgreSQL and create a data base
```shell
git clone https://github.com/Roman28101/cinema-service-api
cd cinema_service_API
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set HOST=<your db host name>
set NAME=<your db name>
set USER=<your db username>
set PASSWORD=<your db password>
set DJANGO_SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run project with docker

Create .env file in main directory (use .env.sample for example)
```shell
docker-compose build
docker-compose up
```


## Get access to project

* Download [ModHeader](https://chrome.google.com/webstore/detail/modheader/idgpnmonknjnojddfkpgkljpfnnfcklj?hl=en)
* create user - /api/user/register
* get access token /api/user/token/



## Features

* JSON Web Token authenticated
* Documentation /api/doc/swagger/
* Creating movies with genres and actors
* Creating cinema halls
* Managing movie tickets and orders
* Filtering movies by date, title
* Filtering movie sessions by title, actors, genres
* Adding movie sessions



## For testing features

You can use this data for testing all the features
```shell
HOST=db
NAME=app
USER=postgres
PASSWORD=supersecretpassword
```
