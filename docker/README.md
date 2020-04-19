# docker

> @TODO: implement this part (fititnt, 2020-04-05 08:28 BRT)

## Uninstall

- See <https://docs.docker.com/engine/reference/commandline/system_prune/>

```bash
# remove all not actively used, except data volumes
docker system prune

# remove all not actively used, EVEN data volumes (be very sure of what you are doing)
docker system prune -a --volumes
```
