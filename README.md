# Dockerized Python Flask API Project

This project demonstrates how to Dockerize a Python Flask API. It will help you set up a simple Flask-based API and run it in a containerized environment using Docker.

## Prerequisites

Before setting up the project, ensure you have the following installed on your machine:

- [Docker](https://www.docker.com/get-started) (for building and running containers)
- [Git](https://git-scm.com/) (for cloning the repository)

## Steps to Set Up

### 1. Clone the repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/Codestaraa/Docker_python_project.git
cd Docker_python_project


2. Build the Docker image
To build the Docker image for this project, run the following command:

bash
docker build -t python-flask-api .

This will create a Docker image with the tag python-flask-api.

3. Run the Docker container
After the image is built, run the container using this command:

bash
docker run -p 5000:5000 python-flask-api
This command maps port 5000 on your local machine to port 5000 inside the Docker container, where the Flask API will be running.

4. Access the API
The Flask API will now be available at http://localhost:5000. You can access it by opening your browser or using curl:

bash
curl http://localhost:5000
This should give you a response from the Flask API.


To stop the running Docker container, use the following command:

bash
docker ps  # Find the container ID
docker stop <container_id>

If you want to remove the container after stopping it:

bash
docker rm <container_id>
Troubleshooting
Ensure that Docker is installed and running on your system.
If you encounter issues while running the commands, check that Docker is correctly set up and the Docker daemon is running.
If port 5000 is already in use, change the port mapping in the docker run command.



