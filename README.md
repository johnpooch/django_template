# Django project template

## Getting started

These instructions will get you started with a copy of the project up on your
local machine for development and testing purposes.

### Docker set up

#### Prerequisites

This set up uses [Docker][docker] and [Docker Compose][docker-compose] for local
development. Follow the docs to get Docker and Docker Compose installed.

#### Bring up local copy

- Run `docker-compose up` to bring up the project (You can run detached by
  adding `-d` flag)
- Once the containers are up you can run commands from inside the docker
  service container by running `docker exec -it django_template_project.web_1`
  and then running whatever command you like.

## Running the tests

From within the service container run `python3 manage.py test`.

### Linting

Run flake8 to check for code style problems. Run `flake8 .` from the project
root. If there are code style problems they will be displayed.

## Test Coverage

To generate a test coverage report test coverage, run `coverage run manage.py test` from within the container. Then run `coverage report` to see the results.

[docker]: https://docs.docker.com/
[docker-compose]: https://docs.docker.com/compose/
