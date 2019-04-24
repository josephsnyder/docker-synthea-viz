# Dockerized Synthetic Patient Visualization instances

## Requirements
This has only been tested using:

* Docker for Windows

## Pre-requisites
A working [Docker](https://www.docker.com/community-edition#/download) installation on the platform of choice.

## Pre-built images
Pre-built images using this repository are available on [docker hub](https://hub.docker.com/r/osehra/)

### Running a Pre-built image
1) Pull the image

    ```
    docker pull osehra/syntheaviz
    ```

2) Run the image

    ```
    docker run -d -p 3080:80 -p 2222:22 --name=syntheaViz osehra/syntheaviz
    ```

## Docker Build

### Build Commands
1) Build the docker image

    ```
    docker build -t syntheaviz .
    ```

2) Run the created image

    ```
    docker run -d -p 3080:80 -p 2222:22P --name=syntheaViz syntheaviz
    ```

Once running, the Synthetic Patient Visualization can be accessed via ```http://localhost:3080/synthea/synthea_upload.php'''