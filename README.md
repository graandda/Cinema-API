# DRF Cinema API

API service for cinema management written on DRF

## Installing using GitHub:

#### Install PostgresSQL and create db

```bash
git clone https://github.com/graandda/Cinema-API.git
cd cinema API
```
```bash
# install requirements
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
```bash
# set your ENV variables
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<vour db user password>
set SECRET_KEY=<your secret key>
```
```bash
# run migrations and server
python manage.py migrate
python manage.py runserver
```
## Run with docker:
#### Docker should be installed
```bash
docker-compose build
docker-compose up
```
## Getting access:
```bash
create user via /api/user/register/
get access token via /api/user/token/
```

## Features:
 * JWT authenticated
 * Admin panel /admin/
 * Documentation is located at /api/doc/swagger/
 * Managing orders and tickets
 * Creating movies with genres, actors
 * Creating cinema halls
 * Adding movie sessions
 * Filtering movies and movie sessions
