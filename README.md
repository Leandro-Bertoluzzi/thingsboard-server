<h1 align="center">Thingsboard server</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/Leandro-Bertoluzzi/thingsboard-server?color=56BEB8">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/Leandro-Bertoluzzi/thingsboard-server?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/Leandro-Bertoluzzi/thingsboard-server?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/Leandro-Bertoluzzi/thingsboard-server?color=56BEB8">
</p>

<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0;
  <a href="#sparkles-features">Features</a> &#xa0; | &#xa0;
  <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0;
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <a href="#memo-license">License</a> &#xa0; | &#xa0;
  <a href="https://github.com/Leandro-Bertoluzzi" target="_blank">Author</a>
</p>

<br>

## :dart: About ##

Setup of ThingsBoard IoT platform ready to go, both for development/testing and production.

In particular, we use ThingsBoard with PostgreSQL as DB and RabbitMQ as message broker. According to docs:

- PostgreSQL as database: [source](https://thingsboard.io/docs/user-guide/install/ubuntu/#step-3-configure-thingsboard-database)
> _ThingsBoard team recommends to use PostgreSQL for development and production environments with reasonable load (< 5000 msg/sec)._

- RabbitMQ as message broker: [source](https://thingsboard.io/docs/user-guide/install/ubuntu/#step-4-choose-thingsboard-queue-service)
>_RabbitMQ is recommended if you don’t have much load and you already have experience with this messaging system._

## :sparkles: Features ##

:heavy_check_mark: Fully featured IoT monitoring system. More info at [ThingsBoard's official docs](https://thingsboard.io/docs/getting-started-guides/what-is-thingsboard/).

## :rocket: Technologies ##

The following tools were used in this project:

- [ThingsBoard](https://thingsboard.io/)
- [RabbitMQ](https://www.rabbitmq.com/)
- [Docker](https://www.docker.com/)

## :white_check_mark: Requirements ##

Before starting :checkered_flag:, you need to have [Git](https://git-scm.com) and [Docker](https://www.docker.com/) installed.

## :checkered_flag: Starting ##

```bash
# 1. Clone this project
$ git clone https://github.com/Leandro-Bertoluzzi/thingsboard-server

# 2. Access the project folder
$ cd thingsboard-server

# 3. Copy and configure the .env files according to your setup
cp rabbitmq.env.dist rabbitmq.env
cp thingsboard.env.dist thingsboard.env

# 4. Run the project with logs
$ docker compose up -d
$ docker compose logs -f thingsboard

# ThingsBoard UI will initialize in <http://localhost:8080>
# RabbitMQ management UI will initialize in <http://localhost:15672>
```

## :memo: License ##

This project is under license from MIT. For more details, see the [LICENSE](LICENSE.md) file.


Made with :heart: by <a href="https://github.com/Leandro-Bertoluzzi" target="_blank">Leandro Bertoluzzi</a>

&#xa0;

<a href="#top">Back to top</a>
