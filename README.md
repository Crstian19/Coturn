# Coturn

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/crstian19/coturn/Docker?style=flat-square)
![Docker Pulls](https://img.shields.io/docker/pulls/crstian/coturn?logo=Docker&style=flat-square)

## Turn/Stun simple server

    docker run -d -p 3478:3478 -p 49160-49200:49160-49200/udp crstian/coturn
    
### Docker-compose


    version: "3.7"
    services:
      coturn:
        container_name: coturn
        image: crstian/coturn
        ports:
          - '3478:3478'
          - '49160-49200:49160-49200/udp'
        restart: always




