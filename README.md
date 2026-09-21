DevOps Status API

A small containerized REST API built as a practical DevOps learning project.

The project demonstrates a simple development-to-CI workflow using Python, Docker, Docker Compose, and GitHub Actions.

Features

* REST API built with Flask
* / endpoint with project status
* /health endpoint for health checks
* Automated tests with pytest
* Docker containerization
* Docker Compose configuration
* GitHub Actions CI pipeline
* Automated Python syntax checks and tests

Technology Stack

* Python 3.12
* Flask
* pytest
* Docker
* Docker Compose
* GitHub Actions

API Endpoints

GET /

Returns basic information about the application.

GET /health

Returns the current health status of the application.

Example response:

{
  "status": "healthy"
}

Running with Docker

Build and start the application:

docker compose up -d --build

The API will be available on:

http://localhost:5000

Running Tests

Install dependencies:

pip install -r requirements.txt

Run the test suite:

pytest

CI/CD

Every push to the main branch and every pull request targeting main triggers a GitHub Actions workflow.

The workflow:

1. Checks out the repository
2. Sets up Python 3.12
3. Installs dependencies
4. Runs the automated test suite

Project Purpose

This project is part of a hands-on DevOps learning path focused on building practical experience with Linux, Git, containers, CI/CD, infrastructure automation, cloud technologies, and networking.

The project is intentionally small so that the complete development and deployment workflow can be understood and extended incrementally.

Future Improvements

Planned improvements include:

* Container health checks
* Image publishing
* Automated Docker image builds
* Deployment to a Linux server
* Infrastructure as Code
* Monitoring and logging
* Additional API functionality
