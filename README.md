# fail2ban-docker

this is a basic repo to store file I use outside the docker-swarm env. Fail2ban is sometimes implemented inside docker image, but when the container is behind a reverse proxy, fail2ban can be ineffective because it is intended to work on table filter and chain INPUT. In this case, the traffic hiting the FORWARD chain is not match against INPUT.

The root dir of fail2ban is considered to be /etc/fail2ban/

Structure :
- /etc/fail2ban/jail.d/custom-dms.conf
- /etc/fail2ban/action.d/docker-traefik-action.conf
- /etc/fail2ban/filter/custom-filter.conf

## TODO :
- install script
- add new custom filters
