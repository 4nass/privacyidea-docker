# PrivacyIdea Docker Image

This is a build environment to build a docker image for privacyIDEA.

## The image
The docker image is a self contained Ubuntu 20.04 with privacyIDEA installed, which will run on every distribution.

## Building

To build the image

```bash
make build
```

## Running

Run it with

```bash
make runserver
```

This will download the existing privacyIDEA container from the Docker hub https://registry.hub.docker.com/u/an455/pricvacy/ and run it.

Login to http://localhost:5000 with "admin"/"privacyidea".

> You must not use this in productive environment, since it contains fixed credentail, encryption keys!

## Advanced usage

### PrivacyIdea Environment variables

- CACHE_TYPE
- PI_PEPPER
- PI_AUDIT_KEY_PRIVATE
- PI_AUDIT_KEY_PUBLIC
- PI_AUDIT_MODULE
- PI_ENCFILE
- PI_EXTERNAL_LINKS
- PI_HSM
- PI_LOGFILE
- PI_LOGLEVEL
- SECRET_KEY
- PI_ADMIN_USER
- PI_ADMIN_PASSWORD

Inspired by https://github.com/tiangolo/uwsgi-nginx-docker
