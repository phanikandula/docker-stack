The contents of this repo were created for meetup presentation "Docker for Full Stack Engineers"
Slides: https://www.phanikandula.com/slides/fullstack-meetup-2/


## Typical workflow with docker-compose

### Validate that the docker-compose.yml file is good:

docker-compose config

### Bring the container up 
This will also build the image first time if you have a Dockerfile. Subsequent docker-compose up won't build the image. Use --build option to force build

docker-compose up -d

### Confirm that the container is 'up':

docker-compose ps

### Connect to the container we brought 'up'
Here 'dev' is name of the service in compose file.

docker-compose exec dev bash 

### Bring the container down once we are done with it.

docker-compose down
