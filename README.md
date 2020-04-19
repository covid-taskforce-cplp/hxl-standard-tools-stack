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

Please note that the @covid-taskforce-cplp obviously are not from the
humanitarian organizations used on this stack and consider using this at your
own risk. **The main objective of this repository is allow more people
test/contribute/use the HXL**.

---

<!-- TOC -->

- [hxl-standard-tools-stack](#hxl-standard-tools-stack)
    - [The Stack](#the-stack)
        - [The HXL stack](#the-hxl-stack)
            - [hxldash](#hxldash)
            - [hxl-proxy](#hxl-proxy)
        - [Non-HXL](#non-hxl)
            - [Portainer](#portainer)
            - [Traefik](#traefik)
    - [Deployment options](#deployment-options)
        - [Docker compose](#docker-compose)
        - [Ansible](#ansible)
    - [Servers](#servers)
        - [Production official servers](#production-official-servers)
        - [Test Server](#test-server)
- [License](#license)

<!-- /TOC -->

---

## The Stack

### The HXL stack
Note: different from most APIs that are maintained by private companies, the
public servers of software related to HXL are hosted by humanitarian
organizations and don't require paid subscriptions, creation of APIs keys, etc.

**If you are doing a project that needs to be used in production and you are not
deploing own private server, don't use our test servers, but these ones**.

#### hxldash
- **Public server**: <https://hxldash.com/>
- **GitHub**: <https://github.com/SimonbJohnson/quickX3>
- **Docker image**<sup>NOT Official</sup>: 
  - GitHub: <https://github.com/covid-taskforce-cplp/hxldash-docker>
  - Docker Hub: <https://hub.docker.com/r/covidtaskforcecplp/hxldash> <sup>May be outdated</sup>

#### hxl-proxy
- **Public server**: <https://proxy.hxlstandard.org/>
- **GitHub**: <https://github.com/HXLStandard/hxl-proxy>
- **Docker image**<sup>Official</sup>: <https://hub.docker.com/r/unocha/hxl-proxy>

### Non-HXL

#### Portainer
- **Public server**: it does not have one (it's interface tool to _watch how the containers are working; great for debugging or deploy non-automated containers_)
- **GitHub**: <https://github.com/portainer/portainer>

#### Traefik
- **Public server**: it does not have one (it's a proxy to _do the HTTPS thing_)
- **Docs**: <https://docs.traefik.io/>
- **GitHub**: <https://github.com/containous/traefik/>

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

- **See [The HXL stack](#the-hxl-stack)**. There you can find servers that can
  be used to host data.

### Test Server

In addition to this repository, for some periodo of active time, we may keep
an live server to use as reference for testing at subdomains from
`hxl.etica.dev`.

See [SECURITY.md](SECURITY.md). You can use this server to make tests and make
suggestions.

- **HXL Dash**
  - <https://dash.hxl.etica.dev/>
- **HXL Proxy**
  - <https://proxy.hxl.etica.dev/>
- **Internal URLs**
  - **Traefik Dashboard**
    - <http://hxl.etica.dev:8888/dashboard/>
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
