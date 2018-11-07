# Light weight docker-compose setup for webapp (nginx, php, mysql)

## What it includes
1. Latest Nginx web server
2. PHP 7.2 FPM
3. MYSQL 5.7

## Requirements
1. `docker` & `docker-compose` installed.

## Configuration steps
1. Clone this repository.
2. Update `docker/nginx/conf.d/template.conf` file:
    * Rename `docker/nginx/conf.d/template.conf` to `your-site.conf`.
    * Change servername as needed.
    * Change root directory as needed.
3. Add hostname to your `etc/hosts` file e.g. `127.0.0.1 your-site.local`.
4. Run command `docker-compose up -d`.
5. Go to browser and enter `your-site.local` and check whether it displays welcome message.

## Development steps
1. Copy your source code to `src/` directory or just start writing in there.
2. Change git remote url to not commit to this repository by `git remote set-url origin Your/Repository`.