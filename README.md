# Quick reference

* Maintained by: [taskbjorn](https://github.com/taskbjorn)
* Official Git repository: [docker-gitea-icongen](https://github.com/taskbjorn/docker-gitea-icongen)

# Supported tags and respective Dockerfile links

* [latest](Dockerfile)

# What is `docker-gitea-icongen`

![Logo](logo.png)

`docker-gitea-icongen` is a Docker container to generate logos and favicons for your self-hosted [Gitea](https://gitea.io) server.

# Running using Docker Compose

Clone this repository to a new folder:

```shell
git clone https://github.com/taskbjorn/docker-gitea-icongen.git
```

Create the input and output folders and copy your favicon and logo to `./input/`:

```shell
mkdir -p input/ output/
cp favicon.svg input
cp logo.svg input
```

Launch the Compose project:

```shell
docker-compose up
```

The Gitea logos and favicons will be generated under `./output/`.

# License

This image is licensed under [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).

As it is often the case with Docker images, some of the software contained in this image (e.g. the base image, software included in the base image, etc.) may be covered under a different license.

Please remember it is your responsibility as the end-user to ensure that your use case complies with the licenses of all included software.