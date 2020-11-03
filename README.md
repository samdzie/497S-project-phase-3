# Team Vision: Project Phase 3

## Overview
Our project is a web application for organizing communities. Our vision
is to combine the features of a home webpage with those of a shared
online calendar. The goal is to allow groups of people - whether they
be friend groups, clubs, or organizations - to have an easy-to-use tool
for organizing events.

This project was developed for [CS 497S: Scalable Web Systems][1], taught by Professor Tim Richards at UMass Amherst in Fall 2020.

## Team Members
- Hichem Bennia
- Sam Dziewietin
- Achintya Kumar
- Angela Nayiga
- Zenry Padua

## System Design
The system is divided into four microservices:

- Web UI: A web app for displaying a group's homepage and calendar.
- Homepages: Manages information displayed on a group's homepage (e.g
group name, welcome message).
- Events: Manages the events displayed on each group's calendar.
- Images: Manages images used by the system, especially group icons.

The Web UI service consists of a frontend and a backend, while the other
services consist of a database and RESTful API. The Web UI frontend
requests data from the backend, which in turn makes API calls over HTTP
to the other services to obtain the necessary data.

Each service is built into a Docker image (or several with
docker-compose). These images are then deployed to AWS Elastic
Beanstalk.

## Scalability
...

## Repositories
- [Web UI](https://github.com/samdzie/group-web-ui)
- [Homepages](https://github.com/HichBen/homepage-api)
- Events
- [Images](https://github.com/Angela-N/image-microservice)

## Demo Video
...


[1]: https://sites.google.com/cs.umass.edu/compsci-497s-f20-submissions
