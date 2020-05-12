---
title: PiHole - A guide
description: This is a post on My Blog about installing pihole.
date: 2020-05-08
tags:
  - blogposts
layout: layouts/post.njk
---
I spent some time instaling [Pi-Hole](https://pi-hole.net/) since I saw that they had v5.0 out on Hacker News.

The last time I had tried it I didn't have as many devices that I would use on my network and uBlock was good enough.

## Docker

I have been using Docker to install a host of things on my raspberry pi 3. I have a media server on there and a few other really cool docker apps in there. Some honorable mentions are Portainer and Watchtower.

So I would use a standard docker run command to install what I wanted but the setup for PiHole required me to set up a macvlan network so I used a docker compose script I found [here](http://tonylawrence.com/posts/unix/synology/free-your-synology-ports/)

1. You need to add the IP address you intend to use on your network to whereever it's mentioned to update.

2. He already has a guide for everything else. Go follow that.

Using docker allows you to keep your installation as is and run pi-hole over everything as opposed to flashing pi-hole to the whole device
