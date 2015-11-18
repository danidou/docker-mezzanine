mezzanine website
=================

## Prerequisites

- Docker Engine
- Docker Compose
- Docker Machine
- docker-paas (ctrlweb)

## Installation

Clone the repository:

```bash
$ git clone https://github.com/CtrlWebInc/docker-mezzanine.git 
```

Then, run:

```bash
$ cd docker-mezzanine && ./initialize_project
$ docker-compose up -d
$ docker-compose run app python manage.py migrate
$ docker-compose stop && docker-compose up -d
```

Woah! That's it! Now if it's morning, pour yourself a coffee. If it's the afternoon, a beer.
The default url for the project is http://mezzanine.local/. You can change it in docker-compose.yml,
and in app/settings.py.
