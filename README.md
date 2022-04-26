# docker_django_postgresql_min

~~~bash
docker-compose up -d
# check web container name
docker ps -a
docker exec -it WEB_CONTAINER_NAME bash

python managa.py migrate auth
python managa.py createsuperuser
# input username and password and not forget these.
python managa.py migrate
python manage.py runserver 0.0.0.0:8000
~~~

access to http://127.0.0.1:8000

or access to http://127.0.0.1:8000/admin
use input username and password to login admin 
