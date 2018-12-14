# Starter kit for theme of Redmine

Starter kit for theme of Redmine.

## Development

### Setup

1. Install [Node.js](https://nodejs.org/en/).js (bundled [npm](https://www.npmjs.com/))
2. Install [Docker](https://www.docker.com/) and [Docker-Compose](https://docs.docker.com/compose/).
3. `git clone https://github.com/akabekobeko/redmine-theme-starter.git`
4. `cd redmine-theme-starter`
5. `npm i`


### Preview on dummy HTML

Transpile (watch) CSS and preview on web browser, this is the local HTML for easy preview without starting Redmine.

* Preview: `npm start`
* Stop: <kbd>Ctrl</kbd> + <kbd>C</kbd>

### Preview on Redmine

Start Redmine and check it.

1. `docker-compose up -d`
2. Access to http://localhost:8080/ on web browser
3. Sign in to Redmine as an administrator
4. Select `mytheme` as the theme from the administration screen.

Stop is `docker-compose stop`.

## License

* [GNU GENERAL PUBLIC LICENSE Version 3](LICENSE)
