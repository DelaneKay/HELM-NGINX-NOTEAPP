# Dockerizing React App with NGINX

This repository demonstrates how to Dockerize a React app with NGINX as the web server. Follow these steps to build and run the Docker image.

## Prerequisites
1. `Docker` installed on your machine.

## Step 1: Clone the Repository
```js
git clone <repository-url>
cd <repository-directory>
```

## Step 2: Create a Dockerfile for React App
Create a Dockerfile named `Dockerfile` in the root directory as in the script above

## Step 3: Build the Docker Image
Build the Docker image by running the following command in the root directory:
```js
docker build -t your-registry/your-react-app-image .
```
Replace your-registry with your Docker registry or username.

## Step 4: Run the Docker Container
Run the Docker container using the following command:
```js
docker run -p 8080:80 your-registry/your-react-app-image
```
This maps port 8080 on your host to port 80 in the Docker container. Adjust the ports as needed.

## Step 5: Access the Application
Open your web browser and navigate to http://localhost:8080 to access the React app served by NGINX.

## Additional Notes
+ If you need to customize NGINX configurations, you can modify the `nginx/nginx.conf` file before building the Docker image.
+ Adjust the Dockerfile and commands based on your specific project structure and requirements.


