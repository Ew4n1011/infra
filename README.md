# Infra

![Available Applications](https://img.shields.io/github/directory-file-count/Ew4n1011/infra/roles?label=Available%20Applications&style=flat-square)
[![license](https://img.shields.io/github/license/DAVFoundation/api_doc.svg?style=flat-square)](https://github.com/Ew4n1011/infra/blob/main/LICENSE)

Docker compose was causing me too many errors, so I decided to swap to ansible. This playbook is heavily inspired by the [ansible-nas](https://github.com/davestephens/ansible-nas) project. Go check it out!

## What Infra does

You can configure Infra to set up any (or all!) of the below on your home or cloud server.

If you have a spare domain name you can configure applications to be accessible externally to your home LAN too; they'll be configured with a sensible hostname and DNS gets updated accordingly if your home IP address changes.

## Available Applications

* [Cloudflare DDNS](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns) - Automatically update Cloudflare with your IP address
* [DDNS Updater](https://github.com/qdm12/ddns-updater) - Dynamic dns updater for several providers
* [Grafana](https://grafana.com) - Query, visualize, alert on, and understand your data no matter where it’s stored (via stats role)
* [Nextcloud](https://nextcloud.com) - A self-hosted Dropbox alternative
* [Portainer](https://portainer.io) - For managing Docker and running custom images
* [Prometheus](https://prometheus.io) - Time series database and monitoring system (via stats role)
* Stats - Monitor and visualise metrics about your machine and internet connection using Grafana, Prometheus, Telegraf and more
* [Traefik](https://traefik.io) - Web proxy and SSL certificate manager

## Preconfigured Application Stacks

Infra application stacks are a number of applications deployed together and preconfigured to perform a common goal.

* Logging - application logging capture and search service based on Grafana Loki.

## What This Could Do

Infra can run anything that's in a Docker image, which is why Portainer is included. A NAS configuration is a pretty personal thing based on what you download, what media you view, how many photos you take...so it's difficult to please everyone.

## What This Doesn't Do

Infra doesn't set up your disk partitions, primarily because getting it wrong can be incredibly destructive. That aside, configuring partitions is usually a one-time (or very infrequent) event, so there's not much to be gained by automating it. Check out the docs(incoming) for recommended setups.

## Installation

Docs to come later

## Documentation

Docs to come later

## Requirements

* Infra targets the latest Ubuntu LTS release, which is currently Ubuntu Server 22.04 LTS.
* You can run Infra on whatever hardware you like, read the docs for more info.

## Getting Help

Getting help is easy! You can:

* Read the docs(to come)
* Start a [discussion](https://github.com/Ew4n1011/infra/discussions)
* Raise an [issue](https://github.com/Ew4n1011/infra/issues) if you think you've found a bug