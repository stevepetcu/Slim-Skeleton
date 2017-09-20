# Dockerized Slim Framework 3 Skeleton Application

Just a Dockerized Slim Framework 3 Skeleton Application.

# Slim Framework 3 Skeleton Application

Use this skeleton application to quickly setup and start working on a new Slim Framework 3 application. This application uses the latest Slim 3 with the PHP-View template renderer. It also uses the Monolog logger.

This skeleton application was built for Composer. This makes setting up a new Slim Framework application quick and easy.

## Install the Application

- Clone this repository.
- Run `$ docker run --rm -v $(pwd):/app slimskeleton_slim_skeleton_composer update`.

## Tests

- Run `$ docker ps | grep slim_skeleton_phpfpm` and note the id in the first column of the corresponding row - the first 3 characters are usually enough. We'll call this the `<phpfpm_container_id>`.
- Run `$ docker exec <phpfpm_container_id> vendor/bin/phpunit` to run the tests.