this docker compose is intended to manage a docker host (or swarm) with shipyard. if you have a swarm, set the constraint to run both containers on the same node. if you have only one local machine, you might point your /var/run/docker.sock within your shipyard-controller instance, and change "-d tcp://" to -d unix:///var/run/docker.sock and omit the --tls* params

you MUST change all <your-...> field within the docker-compose.yaml to make it work!
