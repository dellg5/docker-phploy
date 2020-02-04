# docker-phploy

A Docker container for [PHPloy](https://github.com/banago/PHPloy) that can be used as-is or as a Gitlab-CI docker runner.
[PHPloy](https://github.com/banago/PHPloy) is a command-line tool for deploying a Git Repository over (S)FTP.

How to Build
--------------------

Build from `Dockerfile`:

```sh
docker build --no-cache -t dellg5/phploy .
```

Verify build:

```sh
docker run --rm -it dellg5/phploy phploy
```

Usage
--------------------

1. Install the `dellg5/phploy` container (optional - this step is performed by Docker automatically when running the container):

```sh
docker pull dellg5/phploy
```

2. Run the docker container like this:

```sh
docker run --rm -it -v $(pwd):/app dellg5/phploy phploy
```
