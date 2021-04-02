# laravel-ecr-tutorial
A reference to how I do my Laravel/Apache/MySQL setup using Docker and ECR


## General Overview

1. Build Laravel/PHP & Nginx Docker images locally
2. Push them to ECR
3. Pull them in the docker-compose file, as well as the Docker image for MySQL
4. Run the containers


## Commands WIP
`sudo docker exec -it app_container_name php artisan migrate`
`sudo LE_DIR=./certs docker-compose -f docker-compose.prod.yml up -d`
`sudo docker image rm imagename`

## Caveats
May want to set specific AWS keys with specific permissions for pulling/pushing on ECR repos.
You can do this nicely by making a new policy, this is documented in the `aws` folder.

### Links
https://medium.com/@shakyShane/laravel-docker-part-2-preparing-for-production-9c6a024e9797
