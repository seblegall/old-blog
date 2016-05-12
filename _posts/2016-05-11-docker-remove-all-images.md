---
layout: post
title:  "Docker : Remove all images"
description: "How to remove all images"
date:   2016-05-11 14:49:34
author: Sébastien Le Gall
category: docker
tags: [docker]
---
If you have ever add to work with docker and and docker-compose, you probably often have mistaken in you Dockerfile. Specially when you work with multiple container build from multiple Dockerfile and tag differently.

Here is a simple way to clean all your docker images.

Show images :
{% highlight sh %}
$ docker images
{% endhighlight %}

Delete all container :
{% highlight sh %}
$ docker rm $(docker ps -a -q)
{% endhighlight %}

Delete all images :
{% highlight sh %}
docker rmi $(docker images -q)
{% endhighlight %}
