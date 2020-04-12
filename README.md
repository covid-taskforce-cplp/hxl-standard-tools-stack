# hxl-standard-tools-stack
**Unofficial [IaC](https://en.wikipedia.org/wiki/Infrastructure_as_code) with
[Ansible](https://github.com/ansible/ansible) and
[Docker Compose](https://github.com/docker/compose) stack of selected tools
related to [HXL Standard](https://hxlstandard.org/)**.

> What is HXL? **The Humanitarian Exchange Language**: _HXL is a simple standard
for messy data. Use HXL hashtags to speed up data processing and create
interoperability across data sources. (...) Unlike most data standards, HXL is
cooperative rather than competitive._
<sup>(source: [https://hxlstandard.org/](https://hxlstandard.org/))</sup>

---

<!-- TOC -->

- [hxl-standard-tools-stack](#hxl-standard-tools-stack)
    - [The Stack](#the-stack)
    - [Deployment options](#deployment-options)
        - [Docker compose](#docker-compose)
        - [Ansible](#ansible)
    - [Servers](#servers)
        - [Production official servers](#production-official-servers)
        - [Test Server](#test-server)
- [License](#license)

<!-- /TOC -->

---

This repository is a draft. Please check <https://github.com/covid-taskforce-cplp/hxldash-docker>.

## The Stack

## Deployment options

### Docker compose

- **See [docker/README.md](ansible/README.md)**.

While this repository can deploy a full server using [Ansible](#ansible), we
tried to leave some parts with Docker, so it will more easy to deploy for who
don't want / don't know Ansible.

### Ansible

- **See [ansible/README.md](ansible/README.md)**

Note: the Ansible IaC implementation already will deploy the same docker-compose
files. You are free to use this repository as a base for any private
implementation (the license is flexible, is Public Domain).

## Servers

### Production official servers

- **See [The Stack](#the-stack)**.

### Test Server

At this moment, we're using as test server the `hxl.etica.dev`. **Please do not
add **

- **HXL Dash**
  - <https://dash.hxl.etica.dev/>
- **HXL Proxy**
  - <https://proxy.hxl.etica.dev/>
- **Internal URLs**
  - **Traefik Dashboard**
    - <http://hxl.etica.dev:8080/dashboard/>
    - <https://traefik.hxl.etica.dev/dashboard/>
  - **Portainer**
    - <https://portainer.hxl.etica.dev/> (`admin` : `cplppass`)
  - **whoiam**
    - <https://whoami.hxl.etica.dev/>

# License

[![Public Domain](https://i.creativecommons.org/p/zero/1.0/88x31.png)](UNLICENSE)

To the extent possible under law, the authors of [@covid-taskforce-cplp](https://github.com/covid-taskforce-cplp)
waived all copyright and related or neighboring rights to this work to
[Public Domain](UNLICENSE).
