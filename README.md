# Starter kit for theme of Redmine

Starter kit for theme of Redmine.

## Install

1. Install [Docker](https://www.docker.com/) and [Docker-Compose](https://docs.docker.com/compose/).
2. `git clone https://github.com/akabekobeko/redmine-theme-starter.git`

## Development

1. `docker-compose up -d`
2. Access to http://localhost:8080/ on web browser
3. Sign in to Redmine as an administrator
4. Select `mytheme` as the theme from the administration screen.
5. Make changes to assets/*
6. Reload the web browser and check the screen

If you make a change to src/assets/scss/*, it will be automatically compile SCSS.

Stop is `docker-compose stop`.

## License

- [GNU GENERAL PUBLIC LICENSE Version 3](LICENSE)
