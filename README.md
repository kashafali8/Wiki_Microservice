[![Python application test with Github Actions](https://github.com/nogibjj/Project4_Kashaf/actions/workflows/main.yml/badge.svg)](https://github.com/nogibjj/Project4_Kashaf/actions/workflows/main.yml)
[![AWS CodeBuild](https://codebuild.us-east-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiOHpvOEIvN2VKSS9UaGhJMHRyT25Vd2NjN2tkVHQ5Vno1bm1Sa0hXTWhPTnZ4Q1dORDVoS2tqMkI2cGVTcTQ1K0pMaDlCR1lrWmU3ZnZoUDhGRWg0NDk4PSIsIml2UGFyYW1ldGVyU3BlYyI6Ikh0NThHK3Nyc2R4TDMydWYiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

## Wikipedia Microservice

In this project, I created a Microservice that returns a JSON payload and uses python wikipedia and textblob libraries to perform data engineering task, while employing a cli tool using cli-fire. Later, I also containerised it using Docker and built Continuous Delivery of FastAPI on AWS.

### Project Objectives:

* Create a Microservice that returns a JSON payload and performs a Data Engineering related task
* Push tested source code to Github and perform Continuous Integration with Github Actions (or similar SaaS Build service)
* Build Continuous Delivery of Flask/FastAPI Data Engineering API on AWS

![Project4](https://user-images.githubusercontent.com/111402572/204116175-957d63a4-beeb-4f82-8c1a-03f532bd461b.png)

### Part 1: Initial Setup:

1. Create a python virtual environment in codespaces
2. Create a python Scaffold (Create empty files: 'Makefile', 'requirements.txt', 'main.py', 'Dockerfile', 'mylib/__ init __.py')
3. Populate Makefile
4. Set up Continuous Integration (CI) with Github Actions and also manual checks with 'make lint and make format'

### Part 2: Create a logic Function & Command Line tool using cli-fire:

1. Create a logic function - populated the logic.py file using wikipedia python library
2. Populate the main file by importing functions from the logic file
3. Build a command line tool (cli-fire.py) using python fire library and use chmod +x cli-fire.py to make it executable, and then we can pass it as ./cli-fire.py --help to test the logic.
4. Run the command line tool to test the logic (./cli-fire.py content/phrase/search_wiki/title/url/wiki ...)

### Part 3: Create a FastAPI API:
1. Create a FastAPI API - populated the main.py file using FastAPI library
2. Run the FastAPI API to test the logic
3. Check Swagger documentation

### Part 4: Create a Dockerfile:
1. Create a Dockerfile to package the application and all its dependencies in a virtual container - populated the Dockerfile file using FastAPI library
2. Build the Dockerfile
3. Run the Dockerfile

### Part 5: Deploy with AWS 
1. Create connection with AWS - by adding AWS credntials to Github Secrets
2. Create a fully-managed Docker container registry using ECR which will make it easy to store, manage, and deploy Docker container images.
3. Use AWS CodeBuild to build and test the Docker image (for continuous delivery)



