# Sample-flask-app-with-docker
Sample flask app with docker
In case tag is having the same name already in use
docker rmi my-python-app -f

docker build --tag my-python-app .

In case container is already created with same name so make sure to cleanup using below command
docker container rm -f $(docker container ls -a -q)

docker run --name python-app -p 5000:5000 my-python-app

open browser and see the responce

http://127.0.0.1:5000
