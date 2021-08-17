# react-docker-azure

watch the demo at [https://youtu.be/HCPmNbFW9sQ](https://youtu.be/HCPmNbFW9sQ)

## getting started (for intel based machines)
1. install node modules:

    ```sh
    npm install
    ```
    
2. build the docker container:

    ```sh
    docker build -t <DOCKERHUB_USERNAME>/react-docker-azure:latest .
    ```

3. run the docker container:

    ```sh
    docker run -p 3000:80 <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```

4. navigate to:

    ```sh
    http://localhost:3000
    ```

5. deploy:

    ```sh
    docker push <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```


## getting started (for m1 macs or arm based machines)
1. install node modules:

    ```sh
    npm install
    ```
    
2. build the docker container:

    ```sh
    docker build -f Dockerfile.arm --platform=linux/amd64 -t <DOCKERHUB_USERNAME>/react-docker-azure:latest .
    ```

3. run the docker container

    ```sh
    docker run -p 3000:80 <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```

4. navigate to:

    ```sh
    http://localhost:3000
    ```

5. deploy:

    ```sh
    docker push <DOCKERHUB_USERNAME>/react-docker-azure:latest
    ```
