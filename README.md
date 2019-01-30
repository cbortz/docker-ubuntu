# docker-ubuntu

<!-- [![Docker Repository on Quay.io](https://quay.io/repository/aptible/ubuntu/status)](https://quay.io/repository/aptible/ubuntu) -->
[![Build Status](https://travis-ci.org/cbortz/docker-ubuntu.svg?branch=master)](https://travis-ci.org/cbortz/docker-ubuntu)

Ubuntu base image with custom (originally from [Aptible](https://www.aptible.com)) patches and Dockerfile building tools.

## Installation and Usage

    docker pull quay.io/cbortz/ubuntu
    docker run -i -t quay.io/cbortz/ubuntu

## Available Tags

* `latest`: Ubuntu 16.04 (LTS)
* `16.04`: Ubuntu 16.04 (LTS)

## Included Tools/Patches

* `bats`: The [Bats](https://github.com/sstephenson/bats) Bash Automated Testing System
* `git`: Git Version Control System.
* All Ubuntu LTS security updates (but not non-critical updates).

## Tests

Tests are run as part of the `Dockerfile` build. To execute them separately within a container, run:

    bats test

## Deployment

To push the Docker image to Quay, run the following command:

    make release

## Copyright and License

MIT License, see [LICENSE](LICENSE.md) for details.

Copyright (c) 2019 Chet Bortz and contributors.

---

## Special Thanks

[Frank Macreery](https://github.com/fancyremarker), the great folks at [Aptible](https://www.aptible.com), and all other contributors!

