$ docker network create --attachable --driver overlay --scope swarm keycloak-cluster

$ docker stack deploy --with-registry-auth --compose-file ./mysql-stack.yml mysql

$ docker stack deploy --with-registry-auth --compose-file ./keycloak-stack.yml keycloak
