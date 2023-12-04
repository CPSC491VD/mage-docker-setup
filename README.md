# mage-docker-setup

# Before you attempt this:
Make sure you have followed the steps to deploy the local database.\
The steps to do so can be found at this repository: [Setup local database at localhost](https://github.com/CPSC491VD/setup-local-database).\
Once that is finished, you should have a PostgreSQL instance setup with a ```test_database``` database.

# How to run:
1. Have Docker Desktop installed:  [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Once installed, run the Docker engine (start Docker Desktop)
3. Fetch this repository's code with the download ZIP option
4. cd into the directory that contains the repository and run: `docker compose up --build` to create the image
5. Once finished, access the image at: localhost:6789/
6. Then, follow the instructions at this doc to setup the pipeline code: [Pipeline setup document](https://docs.google.com/document/d/1CYP3d6u2LRaok0DAaRvO_Z8BFEnWxV42EX07rkZ3WGE/edit)