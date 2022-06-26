# BasicPostgresqlDjangoDockerApp
postgresql


step 1: 
```
docker build .
```

step 2:
```
$ docker-compose up -d
```

step 3:
```
docker-compose exec web pipenv install psycopg2-binary==2.8.3
```

step 4:
```
docker-compose exec web python manage.py migrate

docker-compose exec web python manage.py createsuperuser
```
