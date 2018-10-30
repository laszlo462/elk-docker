# Elasticsearch, Logstash, Kibana (ELK) Docker image

## Forked from Sebp's repo in an effort to suit my own deployments.

This Docker image provides a convenient centralised log server and log management web interface, by packaging Elasticsearch, Logstash, and Kibana, collectively known as ELK.

## Changes made from the Spujadas master branch

* Added plugin installation to the deployed image for GeoIP.
* Added 03-opnsense.conf to allow Logstash to correctly make use of syslog output from Opnsense Firewall.
* Docker build now exposes port 5014 UDP/TCP for inbound syslog messages.
* Docker-Compose file updated to reflect deployment on my development rancher environment.

Still need to cleanup this default branch for my usage.  Thanks Spujadas for the great work on your docker repo, this fork has been a great learning experience for me in customizing docker images/builds.

### Documentation

See Sebp's [ELK Docker image documentation web page](http://elk-docker.readthedocs.io/) for complete instructions on how to use his master image.

### Docker Hub

This image is hosted on Docker Hub at [https://hub.docker.com/r/laszlo462/elk-docker/](https://hub.docker.com/r/laszlo462/elk-docker/).
