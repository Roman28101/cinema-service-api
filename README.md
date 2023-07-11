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
set DB_HOST=<your db host name>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db password>
set SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run project with docker

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
DB_HOST=db
DB_NAME=app
DB_USER=postgres
DB_PASSWORD=supersecretpassword
```
