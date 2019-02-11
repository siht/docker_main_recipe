# Recipe for docker django single app

this recipe allows to run a django application without libraries for images or else. Its too simple and only for development

# What do you need

this recipe needs a structure in with three directories:
src, var and etc

## src

contains the projects django itself and here is where have been place settings.py

## etc
contains external files that application doesn't need like requirements.txt

## var
contains external files that provides data like a sql directory

# Settings
you need a .env file or environment vars setted
PROJECT_NAME
POSTGRES_USER
POSTGRES_DB
POSTGRES_PASSWORD
PROJECT_NAME
DJANGO_PORT
SECRET_KEY
DEFAULT_PG_USER
DEFAULT_PG_DB
DEFAULT_PG_PASSWORD

You need to change the vars PROJECT_NAME with the name of the main directory that contains the structure mentioned before.
POSTGRES_USER
POSTGRES_DB
POSTGRES_PASSWORD
are for the postgres admin.
DJANGO_PORT is the output port to connect in a web browser
SECRET_KEY need anything but better a long string
DEFAULT_PG_USER
DEFAULT_PG_DB
DEFAULT_PG_PASSWORD
are for the user of our db (you can repeat the credentials in postgres admin -dont recomended-)

# How to run 

in this example:
## compose
docker-compose up