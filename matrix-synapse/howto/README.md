# Matrix-Synapse
![Network Map of Matrix-Synapse behind Traefik](matrix-telegram-docker.svg)

Matrix synapse has to be started once with the "generate"-command. Run this from your /path/to/my/mydatafolder/matrix-synapse.

## First start: generate the config files
``
  docker run -it --rm \
    -v $PWD/data:/data \
    -e SYNAPSE_SERVER_NAME=your.domain.name \
    -e SYNAPSE_REPORT_STATS=yes \
    matrixdotorg/synapse:latest generate
``