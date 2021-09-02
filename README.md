# HoneyTrap Playground for WSL

This repo contains updated files for the [honeytrap-playground](https://docs.honeytrap.io/manuals/honeytrap-local-playground/) post on their site.

## Setup

### Setup WSL 2 on Windows 10

If you don't have WSL setup on Windows you can follow this [guide](https://docs.microsoft.com/en-us/windows/wsl/install-win10) from Windows. It will walk you through the setup process and how you how to config WSL2, which is needed for the next section

### Setting up Docker Desktop and WSL

You can follow this [guide](https://docs.docker.com/desktop/windows/wsl/) from Docker on how to setup Docker Desktop to use WSL 2 for the backend.


## Quick Start
- clone repo
- drop into wsl `wsl`
- create docker network `docker network create honeytrap`
- create data dir `mkdir data`
- increase the max virtual memory `sudo sysctl -w vm.max_map_count=262144`
- run stack `docker-compose -f docker-compose-honeytrap-playground.yml up`


## Changes
- Update elasticsearch and kibana to lastes version `7.14.0`
- Set elasticsearch discovery type to `single-node`



