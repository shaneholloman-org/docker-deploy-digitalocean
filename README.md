# Docker Deploy to DigitalOcean with Github Actions

This repository contains sample Docker image and GitHub Actions workflow for pushing an image to DigitalOcean container registry.\
The point of this exercise for me is to learn to use other vendor CTLs for image deployment to production and staging servers:

- `awscli`
- `doctl`

Today we will use `doctl` from Digital DigitalOcean. See instructions here: `docs/github/docker-deploy-digitalocean`

## Building

Run `docker build -t sample/my-page .`

## Running

- Run `docker run -it --rm -p 9999:80 --name my-website sample/my-page`
- Open <http://localhost:9999/hello.html>
