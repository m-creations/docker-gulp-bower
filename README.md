docker-gulp-bower
=================

A docker image with the front-end build tools
[Gulp](http://gulpjs.com) and [Bower](http://bower.io),
[Node.js](http://nodejs.org) and [npm](https://www.npmjs.com/) based
on [OpenWRT](http://openwrt.org/).

The minimal size of OpenWRT, which is a distro for embedded devices
make the docker image as small as possible: currently ~ 70 MB.

How to use
----------

The simplest form of usage is:

```
cd ~/myapp

alias mcgb='docker run --rm -it --user=$(id -u):$(id -g) -v `pwd`:/data mcreations/gulp-bower'

mcgb npm install
mcgb bower install
mcgb gulp build

```

You should add the alias statement to your `~/.bashrc`.


Github repo
-----------

https://github.com/m-creations/gulp-bower

Docker Hub
----------

https://registry.hub.docker.com/u/mcreations/docker-gulp-bower/

