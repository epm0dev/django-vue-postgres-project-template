django-vue-postgres-project-template
===========
A project template containing a Dockerized Vue.js application that consumes a Django REST API which uses a PostgreSQL database.

## Project Setup - Development
1. To use this application, you'll need to have [Git](https://git-scm.com/downloads/) and [Docker Compose](https://docs.docker.com/compose/install/) installed on your computer.
2. Then, clone the repository and change to the project directory from your command line as follows:
```
# Clone this repository
git clone https://github.com/epm0dev/django-vue-postgres-project-template

# Change to the repository directory
cd django-vue-postgres-project-template
```
3. Next, create a new file in the project's root directory called `dev.env` and specify values for the following environment variables:
```
SECRET_KEY=
DB_NAME=
DB_USER=
POSTGRES_PASSWORD=
```
4. Then, add the following environment variables and their values to the `dev.env` file you created in the last step:
```
DEBUG=1
ALLOWED_HOSTS=*
CORS_ALLOWED_ORIGINS=http://localhost:8080
```
5. Finally, from your command line:
```
# Build and run the containers for development
docker-compose -f docker-compose.dev.yml up --build
```
