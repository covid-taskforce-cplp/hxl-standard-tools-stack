# docker

See [full-stack/docker-compose.yml](full-stack/docker-compose.yml) for the HXL
main stack.

Note: the [ckan-stack/docker-compose.yml](ckan-stack/docker-compose.yml), with
softwares related to CKAN installed inside docker containers, was a draft and
not used.

## Uninstall

- See <https://docs.docker.com/engine/reference/commandline/system_prune/>

```bash
# remove all not actively used, except data volumes
docker system prune

# remove all not actively used, EVEN data volumes (be very sure of what you are doing)
docker system prune -a --volumes
```
