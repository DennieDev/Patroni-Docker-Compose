# Patroni-Docker-Compose
A very simple PoC setup to test Patroni with Docker Compose and HAProxy

I could not find anything similar so I made this really quickly to test something, I never ended up using Patroni but thought I'd share it for someone else to find. 

Simply build the image and deploy it, to persist the data you should mount something like:

```yaml
    volumes:
      - .../config/patroni.yml:/patroni.yml
      - .../database:/var/lib/postgresql/data
```

