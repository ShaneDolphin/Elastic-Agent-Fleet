# Elastic with Elastic Agent, Fleet, and Elastic APM

This entire thing was built as a solution to the whole certificate sharing thing that happens with Elastic, Logstash, Kibana, and then any applications that you may want to build onto your stack.


### Fleet/Agent

Some things here will not work on Docker Desktop, because you're not going to be able to abstract your binaries locally for the CA part of this. Why? Because Docker Desktop is an emulator, not a real thing. I ran this on Ubuntu 24.04 on AWS EC2 and it worked like a dream.

### Install Docker Engine on Your Ubuntu Instance on EC2:

Docker Stuff:
https://docs.docker.com/engine/install/ubuntu/

Elastic Fleet and Elastic Agent Documentation: https://www.elastic.co/guide/en/fleet/current/fleet-overview.html

## How to make this work

Git clone to your local directory, and then

docker compose up -d

That's it.