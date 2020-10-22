# Deploying react app on NGINX and DOCKER

### About the Project

This project is about how to deploy a react application on nginx and docker.

### Steps
1. Create a React app as per your need
2. Create a ``` Dockerfile ``` on the root level as per this git repo.
3. Create a ``` nginx ``` folder on the root level and a ``` nginx.conf``` file inside it with nginx configuration. This repo just contain the basic configuration.
4. Create a ``` .dockerignore ``` to exclude ``` node_modules ```.
5. Run the command ``` docker build -t [your-container-name] . ``` to build your container
6. Run the command ``` docker run -p 3000:80 [your-container-name] ``` to start the application on port 3000.