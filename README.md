# Flask App with Docker

## About the Project

This is a simple Flask web application that I containerized using Docker.

I practiced building and running the Flask application inside a Docker container on an AWS EC2 Ubuntu instance.

## What I Did

* Cloned a Flask application project for learning.
* Created and modified the `Dockerfile`.
* Used Python 3.11 as the Docker base image.
* Installed Flask and other required Python packages.
* Built a Docker image for the Flask application.
* Created and ran a Docker container.
* Exposed the application using port 80.
* Tested the Flask application from a web browser.
* Used Docker commands to check logs, start, stop, and inspect the container.

## Dockerfile

The Dockerfile contains the instructions to create the Docker image.

The main steps are:

1. Use a Python 3.11 base image.
2. Set `/app` as the working directory.
3. Copy the Flask application files into the container.
4. Install the required Python packages.
5. Run the Flask application.

## Docker Commands

Build the Docker image:

```bash
docker build -t flask-app .
```

Run the container:

```bash
docker run -d -p 80:80 flask-app
```

Check running containers:

```bash
docker ps
```

View container logs:

```bash
docker logs <container-id>
```

Stop the container:

```bash
docker stop <container-id>
```

Start the container again:

```bash
docker start <container-id>
```

## Technologies Used

* Python
* Flask
* Docker
* Linux / Ubuntu
* AWS EC2
* Git
* GitHub

## What I Learned

This project helped me understand the basic Docker workflow:

**Flask Application → Dockerfile → Docker Image → Docker Container**

I also learned how to build and run a Dockerized Flask application on an AWS EC2 Ubuntu server and troubleshoot Docker build errors.

## Learning Source

This project was created as part of my hands-on Docker learning. I used an existing Flask project as a learning example and practiced the Docker setup, configuration, building, and deployment myself.

