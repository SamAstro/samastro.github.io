---
layout: post
title: "Discovering Kafka"
author: "SamAstro"
categories: technologies
tags: [documentation,tutorial]
image: kafka.png
---

## What is Apache Kafka®?
Apache Kafka is a distributed streaming platform capable of handling trillions
of events a day. More on that
[here](https://www.confluent.io/what-is-apache-kafka/).

## How to have Kafka up and running in no time on your computer?
The easiest way to have Kafka up and running is to use Docker.
```bash
$ docker network create kafka-net
$ docker run -d --name zookeeper --network kafka-net zookeeper:3.4.13
$ docker run -d --name kafka --network kafka-net --env ZOOKEEPER_IP=zookeeper ches/kafka
```

## What next?
