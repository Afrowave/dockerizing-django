## Django Development With Docker Compose and Machine

Featuring:

- Docker v20.10.5
- Docker Compose v1.28.5
- Docker Machine v0.16.1
- Python 3.9.0

Blog post -> https://realpython.com/blog/python/django-development-with-docker-compose-and-machine/

### OS X Instructions

1. Start new machine - `docker-machine create -d virtualbox dev;`
1. Configure your shell to use the new machine environment - `eval $(docker-machine env dev)`
1. Build images - `docker-compose build`
1. Start services - `docker-compose up -d`
1. Create migrations - `docker-compose run web python manage.py migrate`
1. Grab IP - `docker-machine ip dev` - and view in your browser
