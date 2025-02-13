---
id: install-with-docker-compose
title: Install with docker-compose
sidebar_label: Install with docker-compose
---

Download Vuls's [docker-compose.yaml](https://github.com/future-architect/vuls/tree/master/setup/docker/)

## install/update all
```console
# docker-compose pull

```

## install/update go-cve-dictionary with docker-compose

```console
# docker-compose pull cve
# docker-compose run  cve -v

go-cve-dictionary v0.1.xxx xxxx
```
## install/update goval-dictionary with docker-compose

```console
# docker-compose pull oval
# docker-compose run oval -v

goval-dictionary v0.1.xxx xxxx
```

## install/update gost with docker-compose

> New version Vuls 0.5.0 now possible to detect vulnerabilities that patches have not been published from distributors using new datasource named [gost](https://github.com/knqyf263/gost).

```console
# docker-compose pull gost
# docker-compose run gost -v

gost  v0.1.xxx xxxx
```

## install/update go-exploitdb with docker-compose

[go-exploitdb](https://github.com/mozqnet/go-exploitdb)
> New version Vuls 0.6.0 now possible to display exploit codes have been published at [Exploit DB.com](https://www.exploit-db.com/). If you don't need to know about exploit code for detected CVEs, skip this section.

```console

# docker-compose pull go-exploitdb

```
go-exploitdb has no Dockerfile TODO.

## install/update Vuls with docker-compose

```console
# docker-compose pull vuls
# docker-compose run  vuls -v

vuls v0.1.xxx xxxx
```

## Scan

See [Tutorial:Docker](tutorial-docker.md)

## How to confirm version and Git revision

- go-cve-dictionary

```console
# docker-compose run  --rm  vuls/go-cve-dictionary -v

go-cve-dictionary v0.0.xxx xxxx
```

- goval-dictionary

```console
# docker-compose run  --rm  vuls/goval-dictionary -v

goval-dictionary v0.0.xxx xxxx
```

- gost

```console
# docker-compose run  --rm  vuls/gost -v

gost v0.0.xxx xxxx
```

- vuls

```console
# docker-compose run  --rm  vuls/vuls -v

vuls v0.0.xxx xxxx
```

## DockerHub

- [vuls/go-cve-dictionary](https://hub.docker.com/r/vuls/go-cve-dictionary/)
- [vuls/goval-dictionary](https://hub.docker.com/r/vuls/goval-dictionary/)
- [vuls/gost](https://hub.docker.com/r/vuls/gost/)
- [vuls/vuls](https://hub.docker.com/r/vuls/vuls/)
- [vuls/vulsrepo](https://hub.docker.com/r/vuls/vulsrepo/) 

This image version is same as the github repository version.
