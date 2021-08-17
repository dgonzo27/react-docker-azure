# react-docker-azure

watch the demo at [https://youtu.be/HCPmNbFW9sQ](https://youtu.be/HCPmNbFW9sQ)

## getting started (for intel based machines)
1. build the docker container:

    ```sh
    docker build -t <DOCKERHUB_USERNAME>/react-docker-azure:latest .
    ```

2. run the docker container:

    ```sh
    docker run -p 3000:80 <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```

3. navigate to:

    ```sh
    http://localhost:3000
    ```

4. deploy:

    ```sh
    docker push <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```


## getting started (for m1 macs or arm based machines)
1. build the docker container:

    ```sh
    docker build -f Dockerfile.arm --platform=linux/amd64 -t <DOCKERHUB_USERNAME>/react-docker-azure:latest .
    ```

2. run the docker container

    ```sh
    docker run -p 3000:80 <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```

3. navigate to:

    ```sh
    http://localhost:3000
    ```

4. deploy:

    ```sh
    docker push <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```
