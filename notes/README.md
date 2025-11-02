## Initial setup:

Edit `Caddyfile`

Edit `docker-compose.yml`

Edit `invenio.cfg`

Create `local-dev.env`

Entry in ORCID:

```
https://fava.local/oauth/authorized/orcid/
```

## Startup

```
docker compose --env-file local-dev.env up
```

In a separate shell, same `cwd`, run the following to setup all the pieces. This takes a while, about 5min or so.

```
docker exec -it invenio-rdm-iplaces-worker-1 setup.sh
```

