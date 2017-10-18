# Storyline
## To run on your local machine

1. Make sure you have Docker and Docker Compose installed
1. Change directory into the root of the project
1. `docker-compose up`
1. Wait for the command to finish then go to http://localhost:8000

## To run migrations or create a new app
1. Make sure the docker containers are running
1. Run `docker ps` to find the Container ID of the web image
1. `docker exec -it [container_id] bash` INSERT THE CONTAINER ID in place of [container_id]
1. From here you can run any python manage.py commands

### Migrations
1. `python manage.py migrate`

### Create app
1. `python manage.py startapp [app_label]`
