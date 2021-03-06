# Internet Utilities

## Connection Utilites

### `aria2`
aria2 is a lightweight multi-protocol & multi-source, cross platform download utility operated in command-line. 

[Github](https://github.com/aria2/aria2)

### `curl`
A command line tool and library for transferring data with URL syntax, supporting HTTP, HTTPS, FTP, FTPS, GOPHER, TFTP, SCP, SFTP, SMB, TELNET, DICT, LDAP, LDAPS, MQTT, FILE, IMAP, SMTP, POP3, RTSP and RTMP.

[Github](https://github.com/curl/curl)

[Manual Page](https://curl.haxx.se/docs/manual.html)

### `openssh`

### `wget`
_Maybe use aria2 or [wget2](https://github.com/rockdaboot/wget2) instead_

[Github](https://github.com/mirror/wget)

### `rclone`
"rsync for cloud storage" 

[Github](https://github.com/rclone/rclone)

### `rsync`
An open source utility that provides fast incremental file transfer. 

[Github](https://github.com/WayneD/rsync)

## Server Stack
### `apache`
### `mariadb`
### `php`

## Services
### `deluge`

[Docker](https://hub.docker.com/r/linuxserver/deluge)

### `heimdall`
An Application dashboard and launcher 

[Git](https://github.com/linuxserver/Heimdall)

[Docker](https://hub.docker.com/r/linuxserver/heimdall)

### `papermerge`
Document management system

[Docker](https://hub.docker.com/r/linuxserver/papermerge)


### `scrutiny`
`smartd` hard drive monitor

[Docker](https://hub.docker.com/r/linuxserver/scrutiny)

### `plex`

[Docker](https://hub.docker.com/r/linuxserver/plex)

Docker:
```
sudo docker create \
  --name=plex \
  --net=host \
  -e PUID=1000 \
  -e PGID=1000 \
  -e VERSION=docker \
  -v /mnt/plexconfig:/config \
  -v /mnt/TV/tv:/tv \
  -v /mnt/Movies:/movies \
  --restart unless-stopped \
  linuxserver/plex
  ```

Docker-compose:
```
---
version: "2.1"
services:
  plex:
    image: linuxserver/plex
    container_name: plex
    network_mode: host
    environment:
      - PUID=1000
      - PGID=1000
      - VERSION=docker
      - UMASK_SET=022 #optional
      - PLEX_CLAIM= #optional
    volumes:
      - /path/to/library:/config
      - /path/to/tvseries:/tv
      - /path/to/movies:/movies
    restart: unless-stopped
```

### `tautuili`
Plex analytics

[Docker](https://hub.docker.com/r/linuxserver/tautulli)



## Downloading

### `sonarr`
TV Downloading

[Docker](https://hub.docker.com/r/linuxserver/sonarr)

### `samba`
[Git](https://gitlab.com/samba-team/samba)

[Docker](https://github.com/dperson/samba)

### `beets`
Audio server

[Docker](https://hub.docker.com/r/linuxserver/beets)

### `airsonic`
Audio streamer

[Docker](https://hub.docker.com/r/linuxserver/airsonic)

### `mcloud`
Music streaming server

[Docker](https://hub.docker.com/r/linuxserver/mstream)

### `booksonic`
Audiobook server

[Docker](https://hub.docker.com/r/linuxserver/booksonic)

## Wiki & KMS

### `raneto`
Knowledge base /Wiki

[Docker](https://hub.docker.com/r/linuxserver/raneto)

### `codimd`
Collective Markdown editor

[Docker](https://hub.docker.com/r/linuxserver/codimd)

### `bookstack`
Wiki

[Docker](https://hub.docker.com/r/linuxserver/bookstack)

## Provisioning
### `ansible`
### `salt`
### `docker`
### `docker-compose`


## Browsers
### `qutebrowser`
### `firefox`

## Remote Desktop Clients

### `remmmina`
Remote desktop client

[Docker](https://hub.docker.com/r/linuxserver/remmina)

### `guacd`
Remote desktop client

[Docker](https://hub.docker.com/r/linuxserver/guacd)

## Filesharing

### `pydio-cells`
[Docker](https://hub.docker.com/r/linuxserver/pydio-cells)

### `nextcloud`
[Docker](https://hub.docker.com/r/linuxserver/nextcloud)

### `syncthing`
[Docker](https://hub.docker.com/r/linuxserver/syncthing)

## Docker Analytics
[Reddit list](https://www.reddit.com/r/docker/comments/j7j915/top_gui_for_docker/)

### `taisun`
Docker desktop monitor

[Docker](https://hub.docker.com/r/linuxserver/taisun)

### `portainer`
Making Docker and Kubernetes management easy. 

[Git](https://github.com/portainer/portainer)

### `ctop`
Top-like interface for container metrics 

[Git](https://github.com/bcicen/ctop)
