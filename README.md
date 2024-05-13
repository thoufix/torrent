Ensure that both the /config and /movies directories are owned by the same user and group, 
and that the user and group correspond to the PUID and PGID values specified in your Docker Compose file.

docker exec -it radarr chown -R 118:65534 /config

docker exec -it radarr chown -R 118:65534 /movies
