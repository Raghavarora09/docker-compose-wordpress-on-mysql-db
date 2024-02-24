# Docker Compose: WordPress on MySQL DB

This repository contains a `docker-compose.yaml` file for setting up WordPress with MySQL database using Docker Compose.

## Steps to Set Up

1. **Create docker-compose.yaml File**: Create a `docker-compose.yaml` file to set up the necessary services and environment.

2. **Define Services and Environment**:
   - Define the version of the Docker Compose file format being used.
   - Define services such as `wordpress` and `mysql`.
   - Specify the image to be used for each service (you can optionally include a tag for the image).
   - In the `wordpress` service, define the `ports` tag for mapping a host port to the container port to run the service.
   - Specify the environment variables such as `host`, `username`, `password`, and `name` for the MySQL service.
   - Use the `volumes` tag to define named volumes that the services use to store persistent data.

3. **Run Docker Compose**: Execute the command `docker-compose up -d` to download the images and run the containers. Use the `-d` flag to run the containers in detached mode.

4. **Check Service Status**:
   - Use the command `curl localhost:8000` to check if the services are running properly (assuming port 8000 is mapped to the WordPress container port 80).
   - Alternatively, open port 8000 directly in another tab of the browser.

5. **Access WordPress**: The WordPress service should be up and running. You can access it through your browser.

6. **Shutdown Service**: To shut down the service, use the command `docker-compose down`.

## Docker Compose File

You can find the `docker-compose.yaml` file in this repository for reference.

Happy containerizing!
