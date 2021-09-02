# Starter kit for theme of Redmine

![Redmine](https://img.shields.io/badge/Redmine-4.2.2-brightgreen)

Starter kit for development theme of Redmine.

## Installation

Please prepare an environment where can use [Node.js](https://nodejs.org/en/), [Docker](https://www.docker.com/) (bundled [Docker Compose](https://docs.docker.com/compose/)), and Git in advance. When are ready, execute the following command.

```
$ git clone https://github.com/akabekobeko/redmine-theme-starter.git
$ cd redmine-theme-starter
$ npm i
```

## Personalization

If you plan to release a theme, replace `mytheme` in the config file below with your own name.

- `package.json`
- `docker-compose.yml`

## Development

### Build

Transpile CSS file from SCSS file.

```
$ npm run build
```

### Watch build for CSS

Invokes a tool that detects changes in the SCSS file and transpile it into the CSS file.

```
$ npm start
```

Stop is <kbd>Ctrl</kbd> + <kbd>C</kbd>.

### Preview on Redmine

Check the theme on Redmine.

#### Preview

```
$ docker-compose up -d
```

1. Access to http://localhost:8080/ on web browser
2. Sign in to Redmine as an administrator
3. Select my theme name as the theme from the administration page
4. Reload the Redmine page in web browser when the theme's SCSS (CSS) file is updated

#### Stop

```
$ docker-compose stop
```

## Release

To release the theme, execute the following command.

```
$ npm run release
```

A theme directory will be generated based on `name` in `package.json`. At the same time, a ZIP archive file with `version` added to the name is generated.

e.g.

- `mytheme`
- `mytheme-1.0.0.zip`

## License

- [GNU GENERAL PUBLIC LICENSE Version 3](LICENSE)
