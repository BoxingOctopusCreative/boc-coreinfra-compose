# boc-coreinfra-compose
Core Infrastructure Compose for Boxing Octopus Creative Services

## Services

### [Traefik](https://traefik.io/traefik)

* Frontend Proxy
* Authenticated by Authelia
* Service defined in [compose/traefik.yaml](./compose/traefik.yaml)

### [Portainer](https://portainer.io)

* Container orchestration frontend
* Service defined in [compose/portainer.yaml](./compose/portainer.yaml)

### [What's Up Docker (aka "WUD")](https://getwud.github.io/wud/#/)

* Container update maintenance
* Service defined in [compose/wud.yaml](./compose/wud.yaml)
* Authenticated by Authelia

### [Authelia](https://www.authelia.com/)

* Auth Service
* Service defined in [compose/authelia.yaml](./compose/authelia.yaml)

### [docker-socket-proxy](https://github.com/Tecnativa/docker-socket-proxy)

* Docker Socket Proxies for WUD, Traefik, Portainer
* Services defined in [compose/wud.yaml](./compose/wud.yaml)