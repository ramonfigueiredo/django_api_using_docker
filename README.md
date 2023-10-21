# Django api using Docker

## Run the API locally

```bash
python3 -m venv venv
source venv/bin/activate
pip3 install --upgrade pip
pip3 install -r requirements.txt
python3 manage.py migrate
python3 manage.py runserver
```

## Run the API using docker

```
docker build -t django_api_using_docker .

docker run -d -p 8080:8080 django_api_using_docker
``` 

or

```
docker build -t django_api_using_docker .

docker run -it -p 8080:8080 django_api_using_docker
```