# Getting Started 2.2

This repository contains projects for the second part of the Tutorial - [Learn to build and deploy your distributed applications easily to the cloud with Docker](https://docker-curriculum.com/)

In this portion of the tutorial, we are going to see how we can run and manage multi-container docker environments with a real-world application which backend is written in Python (Flask) and for search it uses [Elasticsearch](https://www.elastic.co/products/elasticsearch)

To go directly to the tutorial follow the link:

[Docker in MULTI-CONTAINER ENVIRONMENTS](https://docker-curriculum.com/#multi-container-environments)

Note: After a while when you start work with Elastic Container Service, don't forget to follow the [installation procedure of ECS CLI](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ECS_CLI_installation.html); Step 1 and Step 4 would be fine to follow and after that need to follow [ECS CLI Configuration](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ECS_CLI_Configuration.html)- First two steps would be all to follow for this tutorial. In case, if you are wondering how you can create access key for aws, please follow this link [Where’s My Secret Access Key?](https://aws.amazon.com/blogs/security/wheres-my-secret-access-key/) or directly here [Create IAM Users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html#id_users_create_console) and follow some boring steps but carefully.

Below portion is directly copied from the original source to make sure that you have not missed any information:

SF Food Trucks
===

> San Francisco's finger-licking street food now at your fingertips.

![img](shot.png)

This is a fun application built to accompany the [docker curriculum](http://prakhar.me/docker-curriculum) which is a comprehensive tutorial on getting started with Docker targeted especially at beginners. The app is built with [Flask](http://flask.pocoo.org/) on the backend and [Elasticsearch](http://elastic.co/) is the search engine powering the searches. The front-end is built with [React](http://facebook.github.io/react/) and the beautiful maps are courtesy of [Mapbox](https://www.mapbox.com/).

If you find the design of the website a bit ostentatious, blame [Genius](http://genius.com) for giving me the idea of using this color scheme.  Lastly, the data for the food trucks is made available in public domain by [SF Data](https://data.sfgov.org/Economy-and-Community/Mobile-Food-Facility-Permit/rqzj-sfat).

#### Docker

There are two different ways of getting the app up and running with Docker. To learn more how these two differ, checkout the [docker curriculum](http://prakhar.me/docker-curriculum).

##### Docker Network
```
$ ./setup-docker.sh
```

##### Docker Compose
```
$ docker-compose up
```

The app can also be easily deployed on AWS Elastic Container Service. Once you have [aws ecs cli](http://docs.aws.amazon.com/AmazonECS/latest/developerguide/ECS_CLI_installation.html) installed, you can run the following to deploy it on ECS!
```
$ ./setup-aws-ecs.sh
```

Learn more at [docker-curriculum](http://prakhar.me/docker-curriculum).
