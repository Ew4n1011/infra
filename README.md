# Infra

![Available Applications](https://img.shields.io/github/directory-file-count/Ew4n1011/infra/roles?label=Available%20Applications&style=flat-square)
[![license](https://img.shields.io/github/license/DAVFoundation/api_doc.svg?style=flat-square)](https://github.com/Ew4n1011/infra/blob/main/LICENSE)

Docker compose was causing me too many errors, so I decided to swap to ansible. This playbook is heavily inspired by the [ansible-nas](https://github.com/davestephens/ansible-nas) project. Go check it out!

## What Infra does

You can configure Infra to set up any (or all!) of the below on your home or cloud server.

If you have a spare domain name you can configure applications to be accessible externally to your home LAN too; they'll be configured with a sensible hostname and DNS gets updated accordingly if your home IP address changes.

## Available Applications

* [Bazarr](https://github.com/morpheus65535/bazarr) - Companion to Radarr and Sonarr for downloading subtitles
* [Cloudflare DDNS](https://hub.docker.com/r/joshuaavalon/cloudflare-ddns) - Automatically update Cloudflare with your IP address
* [Code Server](https://code.visualstudio.com) - Powerful IDE from Microsoft accessible through the browser
* [DDNS Updater](https://github.com/qdm12/ddns-updater) - Dynamic dns updater for several providers
* [Duplicati](https://www.duplicati.com/) - for backing up your stuff
* [Glances](https://nicolargo.github.io/glances) - For seeing the state of your system via a web browser
* [Grafana](https://grafana.com) - Query, visualize, alert on, and understand your data no matter where it’s stored (via stats role)
* [Guacamole](https://guacamole.apache.org) - Web based remote desktop gateway, supports VNC, RDP and SSH
* [healthchecks.io](https://healthchecks.io) - Ensure your machine is online and get notified otherwise
* [Jellyfin](https://jellyfin.github.io) - The Free Software Media System
* [Jellyseerr](https://github.com/Fallenbagel/jellyseerr) - Open source software application for managing requests for your media library
* [Komga](https://komga.org) - a media server for your comics, mangas, BDs and magazines
* [Lidarr](https://github.com/lidarr/Lidarr) - Music collection manager for Usenet and BitTorrent users
* [Minecraft Server](https://www.minecraft.net) - Server edition of the popular building and exploring game
* [MyMediaForAlexa](https://www.mymediaalexa.com) - Lets you stream your music collection to your alexa device
* [Nextcloud](https://nextcloud.com) - A self-hosted Dropbox alternative
* [Paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) - Scan, index and archive all your physical documents
* [Portainer](https://portainer.io) - For managing Docker and running custom images
* [Prowlarr](https://github.com/Prowlarr/Prowlarr) - Indexer aggregator for Sonarr, Radarr, Lidarr, etc.
* [qBittorrent](https://www.qbittorrent.org) - BitTorrent client
* [Radarr](https://radarr.video) - For organising and downloading movies
* [Route53 DDNS](https://crazymax.dev/ddns-route53) - Automatically update AWS Route53 with your IP address
* [Sonarr](https://sonarr.tv) - For downloading and managing TV episodes
* [Speedtest-Tracker](https://github.com/alexjustesen/speedtest-tracker) - Continuously track your internet speed
* [Prometheus](https://prometheus.io) - Time series database and monitoring system (via stats role)
* Stats - Monitor and visualise metrics about your machine and internet connection using Grafana, Prometheus, Telegraf and more
* [Syncthing](https://syncthing.net) - Sync directories with another device
* [Traefik](https://traefik.io) - Web proxy and SSL certificate manager
* [Vaultwarden](https://github.com/dani-garcia/vaultwarden) - Lightweight Self-Hosting port of Bitwarden password manager, written in Rust
* [Virtual Desktop](https://hub.docker.com/r/linuxserver/rdesktop) - A virtual desktop running on your server
* [Watchtower](https://github.com/containrrr/watchtower) - Monitor your Docker containers and update them if a new version is available
* [YoutubeDL-Material](https://github.com/Tzahi12345/YoutubeDL-Material) - Self-hosted YouTube downloader built on Material Design

## Preconfigured Application Stacks

Infra application stacks are a number of applications deployed together and preconfigured to perform a common goal.

* Media - Mount a media server with sonarr, radarr, bazarr, jellyfin, etc.

## What This Could Do

Infra can run anything that's in a Docker image, which is why Portainer is included. A server configuration can be a pretty personal thing based on what you download, what media you view, how many photos you take...so it's difficult to please everyone.

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