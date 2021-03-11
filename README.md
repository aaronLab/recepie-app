# recipe-app
I'm just playing with Django

## Run

```commandline
docker build .
docker-compose build
docker-compose run app sh -c "python manage.py makemigrations"
docker-compose run app sh -c "python manage.py migrate"
docker-compose run app sh -c "python manage.py runserver 0.0.0.0:8000 --noreload"
```

## Test

```commandline
docker-compose run app sh -c "python manage.py test && flake8"
```
