---
layout: post
title: The programmable datacenter
---

I'm about to build a modern infracture at work. 
And I'll blog about it, mostly to remember what I'm doing and why. 
And to share information with colleagues and the world.  

We'll be running a zeromq broker pushing trader quotes between desks and calibration servers.
A redis server to save the latest broadcast from zeromq and a REST api to access data in redis.  

Also, a database of trades from different trade systems with latest version of the trade. i.e a cache. 
This will be in Cassandra and will have a REST api as well.

All code will be in Python and the different moving parts will be containerized with Docker 
running on top of the programmable datacenter Mesosphere. Except Cassandra that will be deployed as a Mesosphere app. More on that later.


