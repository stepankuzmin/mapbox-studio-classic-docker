# Mapbox Studio Classic Docker image

[![Docker Stars](https://img.shields.io/docker/stars/stepankuzmin/mapbox-studio-classic.svg)]()
[![Docker Pulls](https://img.shields.io/docker/pulls/stepankuzmin/mapbox-studio-classic.svg)]()
[![Docker Automated buil](https://img.shields.io/docker/automated/stepankuzmin/mapbox-studio-classic.svg)]()

[Mapbox Studio Classic](https://github.com/mapbox/mapbox-studio-classic) is a desktop application for vector tile driven map design.

![Screenshot](https://raw.githubusercontent.com/stepankuzmin/mapbox-studio-classic-docker/master/screenshot.png)

## Usage

```shell
docker run -d -p 3000:3000 stepankuzmin/mapbox-studio-classic
```

You can also mount a host directory as a data volume:

```shell
docker run -d \
  -p 3000:3000 \
  -v /data:/root \
  --name studio \
  stepankuzmin/mapbox-studio-classic
```

This command mounts the host directory, `/data`, into the container at `/root`.

## Getting started

The docs offer both a step-by-step guide to creating your first projects in Mapbox Studio Classic and detailed information about styling and creating vector sources.

- [Style quickstart](https://www.mapbox.com/help/style-quickstart/)
- [Source quickstart](https://www.mapbox.com/help/source-quickstart/)
- [Common questions](https://www.mapbox.com/help/studio-common-questions/)
- [Contributing to Mapbox Studio Classic](https://github.com/mapbox/mapbox-studio-classic/blob/mb-pages/CONTRIBUTING.md)
