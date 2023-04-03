# Cinema-API

API service for cinema management written on DRF

## Installing using GitHub

Install PostgresSQL and create db

```shell
git clone https://github.com/Tania-Kharchuk/cinema_API
cd cinema_API
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
export DB_HOST=<your db hostname>
export DB_NAME=<your db name>
export DB_USER=<your db username>
export DB_PASSWORD=<your db user password>
export SECRET_KEY=<your secret key>
python manage.py migrate
python manage.py runserver
```

## Run with Docker

Docker should be installed

```shell
docker-compose build
docker-compose up
```

## Getting access

* create user via api/user/register
* get access token via api/user/token

## Features

* JWT authenticated
* Admin panel /admin/
* Documentation is located at /api/doc/swagger/
* Managing orders and tickets 
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions
