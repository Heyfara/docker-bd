# Docker Symfony (MySQL - ELK)

Simple docker setup to run a Mysql database. Also comes with an elk stack to display logs.
Based on [Docker-Symfony](https://github.com/maxpou/docker-symfony)

## Installation

1. Create a `.env` from the `.env.dist` file. Adapt it according to your symfony application

    ```bash
    cp .env.dist .env
    ```


2. Build/run containers with

    ```bash
    $ docker-compose build
    $ docker-compose up -d
    ```

3. Prepare Symfony app
    1. Update your db config

        ```yml
        # path/to/your/symfony-project/.env
            DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/db_name
        ```

## Usage

Just run `docker-compose up -d`
