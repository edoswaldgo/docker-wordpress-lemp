# WordPress LEMP Starter Project via Docker

A WordPress starter project that uses Docker Compose for quickly setting up your environment. This project uses [LEMP](https://lemp.io/) stack which composed of Nginx, MariaDB, WordPress v4.9.8, and PHP-FPM v7.2.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Installing

1. Install Docker and Compose. Click [here](https://docs.docker.com/install/) for the official guide.

2. Clone this Git repository.

    ```
    git clone https://github.com/edoswaldgo/docker-wordpress-lemp.git
    ```

3. Run Docker Compose

    ```
    cd docker-wordpress-lemp
    docker-compose up -d
    ```

4. Open the URL ( [http://localhost](http://localhost) ) via web browser for initial WordPress setup.

5. Voila! Your environment is up and running.

### Project Structure

``` ANSI
docker-wordpress-lemp
+-- db-data
+-- logs
+-- nginx
|   +-- wordpress.conf
+-- wordpress
|   +-- ...
+-- docker-compose.yml
```

* `db-data` folder is the mounted volume for MariaDB persistence. 
* `logs` folder contains the logs of the Nginx container.
* `nginx/wordpress.conf` is the default Nginx config for PHP-FPM integration.
* `wordpress` folder is your usual project inside `htdocs`.
    * Note: WordPress Core and Uploads are not included in this Git project.
* `docker-compose.yml` is the Docker Compose config file for running the LEMP stack.

## Contributing

1. Fork the Git project ( https://github.com/edoswaldgo/docker-wordpress-lemp )
2. Create your issue branch ( `git checkout -b fix/xxxxx` )
3. Commit your changes ( `git commit -m "Fix issue xxxxx: <Commit Details Here>"` )
4. Push your branch to origin ( `git push` )
5. Create a pull request.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/edoswaldgo/docker-wordpress-lemp/tags). 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
