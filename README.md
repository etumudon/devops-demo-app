# Node.js CI/CD Demo App

## Objective

This project demonstrates a complete CI/CD pipeline for a Node.js web application using GitHub Actions and Docker.

## Tools Used

* Node.js
* Express.js
* Docker
* GitHub
* GitHub Actions
* Docker Hub

## CI/CD Workflow

The workflow is triggered automatically whenever code is pushed to the `main` branch.

The pipeline performs the following steps:

1. Checks out the source code.
2. Sets up the Node.js environment.
3. Installs project dependencies.
4. Runs the test script.
5. Builds a Docker image.
6. Logs in to Docker Hub using GitHub Secrets.
7. Pushes the Docker image to Docker Hub.

## Project Structure

* `server.js` – Main application file
* `Dockerfile` – Docker image configuration
* `.github/workflows/main.yml` – GitHub Actions workflow
* `package.json` – Project dependencies and scripts

## Running the Project Locally

Install dependencies:

```bash
npm install
```

Start the application:

```bash
npm start
```

Build the Docker image:

```bash
docker build -t devops-demo-app .
```

Run the Docker container:

```bash
docker run -p 3000:3000 devops-demo-app
```

Open your browser and visit:

`http://localhost:3000`

## Outcome

The project successfully automates testing, Docker image creation, and Docker Hub deployment using GitHub Actions, demonstrating a complete CI/CD pipeline.
