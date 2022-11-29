---
title: "How to proxy Docker container directly with Nginx Proxy Manager"
date: 2022-11-20T09:03:20-08:00
draft: false
tags: ['docker', 'nginx proxy manager', 'dev', 'server', 'proxy']
---
## Introduction

When exposing services to the internet, it can be a good idea to not directly expose the ports, but to use a reverse proxy. Especially when hosting multiple services under one domain, this can become pretty handy. 

A tool i like to use is the Nginx Proxy Manager, which is a graphical user interface to use Nginx as a reverse proxy. When doing so with services running one my Homelab in my private network, im used to map the container port to the docker host port and then use the internal network ip's as the forward goal in the reverse proxy. This works fine but you don't always have a network configuration like this.
