# n8n Docker

- running docker inline without a docker compose

``` sh
docker run -d --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  -e N8N_BASIC_AUTH_ACTIVE=true \
  -e N8N_BASIC_AUTH_USER=admin \
  -e N8N_BASIC_AUTH_PASSWORD=admin \
  n8nio/n8n
```

- running docker compose

``` sh
docker-compose up -d
```

- open n8n 

```
http://localhost:5678
```