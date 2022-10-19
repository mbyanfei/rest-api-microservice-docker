# https://dev.to/swarnimwalavalkar/build-and-deploy-a-rest-api-microservice-with-python-flask-and-docker-5c2d
# rest-api-microservice-docker
An example of a RESTful API Deployed on a Docker Container

docker build -t flaskbookapi:1.0 .

docker run -p 5000:5000 --name FlaskBookAPI flaskbookapi:1.0


curl --header "Content-Type: application/json"  --request POST  --data '{"title":"yan title","author":"yan","length":200,"rating":5.0}'  http://localhost:5000/books

curl --header "Content-Type: application/json"  --request DELETE  http://localhost:5000/books/4

in brower: 
https://mbyanfei-rest-api-microservice-docker-qx5qx69jjj2xprr-5000.githubpreview.dev/books


