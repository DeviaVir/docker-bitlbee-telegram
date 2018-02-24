docker-bitlbee-telegram
==============

This repo provides the steps necessary to build a
[BitlBee](http://www.bitlbee.org/) docker image.

This bitlbee includes libpurple

Docker registry
---------------

This image is available at: [hub.docker.com/r/deviavir/docker-bitlbee-telegram/](https://hub.docker.com/r/deviavir/docker-bitlbee-telegram/)

Build manually
--------------

```
$ git clone https://github.com/deviavir/docker-bitlbee-telegram
$ docker build --rm -t deviavir/bitlbee-telegram .
```

Running
-------

It exposes port 6667 and use volume /var/lib/bitlbee for configuration files.

```
$ docker run -d --name=bitlbee-telegram -v /var/volumes/bitlbee-telegram:/var/lib/bitlbee/ deviavir/bitlbee-telegram
```
