# Postgresql & PgAdmin

Quickly start Postgresql and PgAdmin for development

## Configuration

- if you're running psql as a service or mapping its port change the port mapping for the `psql` service in the docker-compose.yaml file
- if yuo're running something on port 8080 change the port for the `pgadmin` service to something else in the docker-compose.yaml file

## Usage

- docker-compose up
- go to http://localhost:8080 use user: `test@test.com` and password: `4321test.`
  - connect to the database by adding a server with host: `psql` user: `root` password: `root`
- volumes are configured for both psql and pgadmin so you can keep your data between restarts
