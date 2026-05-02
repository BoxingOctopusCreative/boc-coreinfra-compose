# boc-coreinfra-compose
Core Infrastructure Compose for Boxing Octopus Creative Services

## Introduction

* Core services for Boxing Octopus Creative
* All services served on subdomains under `boxingoctopus.io`

## Services

### [Traefik](https://traefik.io/traefik)

* Frontend Proxy
* Dashboard located @ https://traefik.boxingoctopus.io
* Authenticated by Authelia
* Service defined in [compose/traefik.yml](./compose/traefik.yml)

### [Portainer](https://portainer.io)

* Container orchestration frontend
* UI located @ https://portainer.boxingoctopus.io
* Service defined in [compose/portainer.yml](./compose/portainer.yml)

### [What's Up Docker (aka "WUD")](https://getwud.github.io/wud/#/)

* Container update maintenance
* Dashboard located @ https://wud.boxingoctopus.io
* Service defined in [compose/wud.yml](./compose/wud.yml)
* Authenticated by Authelia

### [Authelia](https://www.authelia.com/)

* Auth Service
* UI located @ https://auth.boxingoctopus.io
* Service defined in [compose/authelia.yml](./compose/authelia.yml)

### [docker-socket-proxy](https://github.com/Tecnativa/docker-socket-proxy)

* Docker Socket Proxies for WUD, Traefik, Portainer
* Services defined in [compose/wud.yml](./compose/wud.yml)