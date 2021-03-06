[![Build Status](https://travis-ci.org/F5Networks/marathon-bigip-ctlr.svg?branch=master)](https://travis-ci.org/F5Networks/marathon-bigip-ctlr) [![Coverage Status](https://coveralls.io/repos/github/F5Networks/marathon-bigip-ctlr/badge.svg?branch=HEAD)](https://coveralls.io/github/F5Networks/marathon-bigip-ctlr?branch=HEAD)

F5 BIG-IP Controller for Marathon
=================================

The F5 BIG-IP Controller for Marathon makes F5 BIG-IP
[Local Traffic Manager](https://f5.com/products/big-ip/local-traffic-manager-ltm)
services available for applications defined in a
[Marathon](https://mesosphere.github.io/marathon/) environment.

Documentation
-------------

For instruction on how to use this component, see the
[docs](http://clouddocs.f5.com/products/connectors/marathon-bigip-ctlr/latest/) for
F5 BIG-IP Controller for Marathon.

For guides on this and other solutions for Marathon, see the
[F5 Marathon Solution Guides](http://clouddocs.f5.com/containers/latest/marathon).

Running
-------

The official docker image is `f5networks/marathon-bigip-ctlr`.

Usually the controller is deployed in Marathon. However, the controller can be run locally for development testing.

```shell
docker run f5networks/marathon-bigip-ctlr <args>`
```

Building
--------

Note that these instructions will only work for internal users.

To checkout and build:

```shell
git clone https://github.com/f5networks/marathon-bigip-ctlr.git
cd marathon-bigip-ctlr
```

To build the docker image:

```shell
docker build -t IMG_TAG .
```

To build a docker image with those artifacts:

```shell
./build-tools/build-runtime-image.sh
```
