# CST8915 Lab 4 - Introduction to Docker

## Demo Video

YouTube Link: [https://youtu.be/dhQTPsGvffk]

## Reflection Questions

### 1. What are the main differences between a Docker image and a Docker container?

A Docker image is a read-only template that contains the application and everything needed to run it, such as dependencies and configuration. A Docker container is a running instance created from an image. One image can be used to create multiple containers.

### 2. Explain how Docker's layered architecture improves efficiency.

Docker images are made of different layers. These layers can be reused and shared between images and containers instead of creating the same files again. This helps save storage space and makes building and starting containers more efficient.

### 3. Why does each container get its own writable layer?

The image layers are read-only, so each container needs its own writable layer to store changes made while it is running. This also allows multiple containers to use the same image without changing the original image or affecting each other.

### 4. What are the benefits of using Docker Compose over running containers individually?

Docker Compose makes it easier to manage multiple containers together using one YAML file. In this lab, I used Docker Compose to manage the web application and Redis service together. It also made it easier to start, stop, restart, and scale the services using simple commands.
