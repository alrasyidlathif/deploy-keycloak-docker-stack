$ docker network create --attachable --driver overlay --scope swarm keycloak-cluster

$ docker stack deploy --with-registry-auth --compose-file ./docker-stack.yml keycloak
