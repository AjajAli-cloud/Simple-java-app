# Simple Java Docker

A beginner-friendly Java application running inside a Docker container.

## Project Overview

This project demonstrates how to:

* Create a simple Java application
* Create a Dockerfile
* Build a Docker image
* Run a Docker container
* Understand the basic Docker workflow

## Project Structure

```text
simple-java-docker/
├── Main.java
├── Dockerfile
├── README.md
└── .gitignore
```

## Technologies Used

* Java 17
* Docker
* Dockerfile
* Git
* GitHub

## Java Application

The application prints a simple message:

```text
Hello from Java Docker!
My first Java application running inside Docker.
```

## Dockerfile

The Dockerfile uses Eclipse Temurin Java 17:

```dockerfile
FROM eclipse-temurin:17-jdk

WORKDIR /app

COPY Main.java .

RUN javac Main.java

CMD ["java", "Main"]
```

## Build Docker Image

Open the terminal inside the project directory and run:

```bash
docker build -t java-app .
```

## Run Docker Container

Run the container:

```bash
docker run java-app
```

Expected output:

```text
Hello from Java Docker!
My first Java application running inside Docker.
```

## Run Temporary Container

To automatically remove the container after it exits:

```bash
docker run --rm java-app
```

## Check Docker Images

```bash
docker images
```

## Check Containers

```bash
docker ps -a
```

## Git Commands

Initialize Git:

```bash
git init
```

Add project files:

```bash
git add .
```

Create a commit:

```bash
git commit -m "Add simple Java Docker project"
```

Push the project to GitHub:

```bash
git push -u origin main
```

## Learning Outcome

This project provides hands-on practice with the basic Docker workflow:

```text
Java Code
    ↓
Dockerfile
    ↓
Docker Image
    ↓
Docker Container
    ↓
Application Output
```

## Author

Ajaj Ali

BTech CSE | Cloud & DevOps Learner
