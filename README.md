# komodo
running komodo with least privs and secrets please mind the change:
```
      dockerfile_inline: |
        FROM ghcr.io/moghtech/komodo-periphery:${COMPOSE_KOMODO_IMAGE_TAG:-latest}
        USER 1000:1000
        WORKDIR /home/<USER>
        ENV HOME=/home/<USER>
```
