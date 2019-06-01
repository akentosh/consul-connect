# Consul Connect Simple Echo Demo

    docker run -ti --rm --network host consul:latest intention create -deny client echo
    docker run -ti --rm --network host gophernet/netcat localhost 9191
    docker run -ti --rm --network host consul:latest intention delete client echo
    docker run -ti --rm --network host gophernet/netcat localhost 9191
