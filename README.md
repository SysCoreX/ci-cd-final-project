# CI/CD Final Project

**Project name:** ci-cd-final-project – CI/CD pipeline with GitHub Actions, Tekton and OpenShift

This repository contains my final project for the Coursera course **CI/CD Tools and Practices**.
It applies CI/CD concepts to a sample Python (Flask) application.

## Pipeline overview

- **GitHub Actions** – lint with flake8 and run unit tests with nose on every push and pull request
- **Tekton** – tasks for cleanup, linting (flake8) and unit testing (nose)
- **OpenShift Pipelines** – automated pipeline that builds and deploys the application to an OpenShift cluster

## Repository structure

- `.github/workflows/workflow.yml` – GitHub Actions workflow
- `.tekton/tasks.yml` – Tekton tasks (cleanup, flake8, nose)
- `service/` – application source code
- `tests/` – unit tests
- `Dockerfile` – container image definition

## Setup

After entering the lab environment, run the `setup.sh` script in the `./bin` folder to install the prerequisite software.

```bash
bash bin/setup.sh
```

Then exit the shell and start a new one for the Python virtual environment to be activated.

```bash
exit
```

## License

Licensed under the Apache License. See [LICENSE](/LICENSE)

## Author

Kristof Muhari
