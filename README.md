Usenet Docker
Containers
[linuxserver/sabnzbd](https://github.com/linuxserver/docker-sabnzbd) - SABnzbd
[plexinc/plex](https://hub.docker.com/r/plexinc/pms-docker) - Plex
[linuxserver/sonarr](https://github.com/linuxserver/docker-sonarr) - Sonarr
[linuxserver/radarr](https://github.com/linuxserver/docker-radarr) - Radarr
[netdata/netdata](https://hub.docker.com/r/netdata/netdata) - Netdata
[portainer/portainer](https://hub.docker.com/r/portainer/portainer) - Portainer
[phpmyadmin/phpmyadmin](https://hub.docker.com/r/phpmyadmin/phpmyadmin/) - PHPMyAdmin
[linuxserver/mariadb](https://hub.docker.com/r/linuxserver/mariadb) - MariaDB
[v2tec/watchtower](https://hub.docker.com/r/v2tec/watchtower) - Watchtower

# Docker Setup

1. Set `PLEX_CLAIM` from https://www.plex.tv/claim/ in compose file along with proper `ADVERTISE_IP` of Docker host.
2. Configure `/etc/environment` with `UID` (`PUID`) and ``GID` (`PGID`) of user with access to TV/Movie/Download directories exposed to Docker containers along with `TZ`, `USERDIR` and any password you want to use for MariaDB with `MYSQL_ROOT_PASSWORD`.
3. Run `docker-compose up -d` to start all the associated service containers.
