# Git and Docker Starter Application

This repository contains a small Python web application used to practice Git, GitHub, and Docker workflows.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

The running application should be verified using an HTTP request to port 8000.

## Usage
This command builds the image and tags it with test using context in the current directory.

    docker build -t git-docker-app:test .

This command runs the container in detached mode with the name app-test.
8080:8000 maps the local port to port 8000.
the final part is the image you built earlier.


    docker run -d --name app-test -p 8080:8000 git-docker-app:test

This command sends a get request to port 8000 and should respond with 200 if everything works.

    curl localhost:8080
## Conflict A AND Conflict B

