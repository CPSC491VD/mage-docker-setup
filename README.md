# mage-docker-setup

# Read this before attempting:
Make sure you have followed the steps to deploy the local database.\
The steps to do so can be found at this repository: [Setup local database at localhost](https://github.com/CPSC491VD/setup-local-database).\
Once that is finished, you should have a PostgreSQL instance setup with a ```test_database``` database.
\
\
Additionally, you should have started up pgAdmin and connected to the PostgreSQL 16 server by right clicking on PostgreSQL16 and selecting ```connect server```. You should use the password you set during the installation of PostgreSQL 16. \
![PostgreSQL 16 Server](images/psql_server.png)


# How to run:
1. Have Docker Desktop installed:  [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Once installed, run the Docker engine (start Docker Desktop)
3. Fetch this repository's code with the download ZIP option, then extract the zip into your working directory.
4. Set your correct PostgreSQL password in the included .env file. \
For example, if your PostgreSQL password was ```abc123``` you would change ```POSTGRES_PASSWORD=postgres``` to be ```POSTGRES_PASSWORD=abc123```
5. cd into the directory that contains the repository and run: `docker compose up` to create the image. If successful, you should see your container appear on the Docker Desktop application: ![Container](images/docker_container.png)
6. Once finished, access the image at: localhost:6789/
7. Assuming you have everything correctly setup, including the local sample database, you can locate the pipeline under the ```pipelines``` page and click on its name. Then you can select run once to run the pipeline once.

![Running the pipeline once](images/run_once.png)