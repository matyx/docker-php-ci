# PHP CI Docker images

This repository contains Docker images for PHP 5.6 and higher which are based on the [official PHP Docker images](https://hub.docker.com/r/_/php/). These images were created specifically to use them for continious integration (Gitlab CI specifically), but they can be used for other purposes too.

These images contain the following additions to the vanilla PHP images:

* Version control packages (git, mercurial, subversion)
* nodejs, npm, bower
* composer
* deployer
* PHP extensions:
   * curl
   * gettext
   * intl
   * json
   * mcrypt
   * mbstring
   * mysqli
   * opcache
   * pdo_mysql
   * soap
   * xsl
   * zip
   * gd
   * intl


## Pull images

The images are stored on [Docker Hub](https://hub.docker.com/r/packetery/ci/). Use `docker pull packetery/ci` to pull these images.

The following tags are available:

* 5.6
* 7.0
* 7.1

## Build process

The Dockerfiles are stored in directories for each image version. Docker Hub builds new images automatically when this repository or the PHP base images are updated.

## License

The Dockerfiles are licensed under the MIT license, see LICENSE for details.

