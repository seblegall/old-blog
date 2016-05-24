---
layout: page
title:  "About Me"
description: "Sébastien Le Gall"
date:   2016-05-11 14:49:34
author: Sébastien Le Gall
---

Hi ! I'm a french software engineer working at Kilix, a great web agency. I feel passionate by Symfony 3 and PHP7 developement.

I also manage some projects development with Agile methods based on multiple framework such as SCRUM, Kanban and eXtrem Programming.

Here are some of the tools I like to use :

* Docker
* Ansible
* PHP7
* Emacs
* Symfony

You can find a few of my personal projects I like to use at work cin the next sections.

## My Github projects

### Emacs for Symfony

[https://github.com/seblegall/emacs-symfony2](https://github.com/seblegall/emacs-symfony2)

Working with the Symfony framework is great. Unless you loose to much time to find your PHP files and change folders by clicking on this very little "+" that allows you to see the folders tree... Choose the best editor. Choose Emacs.

Here is my Emacs configuration to use with all kind of PHP project and specially with Symfony2 based project.

### PHP7.0 web app Docker environment

[https://github.com/seblegall/php7-web-app-docker-env](https://github.com/seblegall/php7-web-app-docker-env)

Provide a full PHP7.0 - Nginx development environment using docker and docker-compose.

### A Bash Script boilerplate

[https://github.com/seblegall/bash-script-options-boilerplate](https://github.com/seblegall/bash-script-options-boilerplate)

Yet another bash script with option boilerplate offering :

* Interactive mode
* Quiet mode
* CLI options parser supporting -n --name --name=Oxy --name Oxy
* Bundling of flags. ie. -vf instead of -v -f
* Helper functions for printing messages such as success and error
* Automatically remove color escape codes if the script is piped.


## My Docker container

### A PHP docker container

[https://hub.docker.com/r/seblegall/php-docker/](https://hub.docker.com/r/seblegall/php-docker/)

A basic docker container running PHP 7.0 or PHP 5.6.
This container is useful when running simple php script.

### A PHP-Cli docker container

[https://hub.docker.com/r/seblegall/php-cli-docker/](https://hub.docker.com/r/seblegall/php-cli-docker/)

A docker container running PHP 7.0 or PHP 5.6 command line tools.
This container let you run PHP-cli scripts and use much more tools such as Capistrano, GruntJS, Gulp, Bower, Mysql client, etc.
It is design to be run as a daemon and then, let you execute a bash shell. In this shell you will be able to use all tools you need to commit your code, compile assets, deploy, etc.
