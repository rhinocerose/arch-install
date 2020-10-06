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
### `plex`

[Docker](https://hub.docker.com/r/linuxserver/plex)

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
### `samba`
[Git](https://gitlab.com/samba-team/samba)

[Docker](https://github.com/dperson/samba)


## Provisioning
### `ansible`
### `salt`
### `docker`
### `docker-compose`
### `portainer`
Making Docker and Kubernetes management easy. 

[Git](https://github.com/portainer/portainer)

## Browsers
### `qutebrowser`
### `firefox`