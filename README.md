# Full-Stack Application: React, Django, MySQL with Docker Compose

## Overview

This repository contains a full-stack web application built with React for the frontend, Django for the backend, and MySQL as the database, all orchestrated using Docker Compose.

### Features

- Frontend built with React, providing a user-friendly interface.
- Backend powered by Django, offering RESTful API endpoints.
- MySQL database for storing application data.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)  
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

### Clone the Repository

### Running the Application
1. Navigate to the `backend` folder and build the image:
   ```bash
   docker build -t django-image:latest .
   ```

2. Move to the `frontend` folder and build the image:
   ```bash
   docker build -t react_img:latest .
   ```

3. Return to the root folder and run the command:
   ```bash
   docker-compose up -d
   ```
### Additional Information
#### Points to Note:
- Customize Dockerfiles and configurations for individual services as required.
- Ensure alignment of React and Django configurations with the Docker services and network setups specified in docker-compose.yml.
- Persistent data storage for the MySQL service is maintained in the ./mysql directory. Modify the volume mount as needed.
