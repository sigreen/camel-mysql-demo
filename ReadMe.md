Sample Camel MySql Integration Project
===========================

## Prerequisites

1. Install MySql Server
2. Create the Shop table described [here](https://dev.mysql.com/doc/refman/5.6/en/examples.html)

## Run locally

To build this project use

    mvn install

To run this project with Maven use

    mvn camel:run

## Running on JBoss Fuse

Install MySql driver in Fuse with:

> osgi:install -s wrap:mvn:mysql/mysql-connector-java/5.1.39

Install into Fuse with:

> features:addurl mvn:com.redhat/camel-mysql-demo/1.0.0/xml/features

> features:install camel-mysql-demo

And you can see the application running by tailing the logs

> log:tail

And you can use ctrl + c to stop tailing the log.

