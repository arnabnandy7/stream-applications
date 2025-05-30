## Stream Applications

In this repository, you will find a collection of components that can meet various data integration use cases and requirements.

The repository's primary focus is to provide a set of standalone Java functions that can be useful in the end-user
applications as-is.

Besides, this repository builds on the Java functions to generate standalone Spring Cloud Stream applications that can run
against Spring Cloud Stream's RabbitMQ or Apache Kafka binder implementations. It is also possible to extend the generator
to bundle the Java functions with the other supported binder implementations.

These applications can run standalone or as part of a data flow, such as the one orchestrated using Spring Cloud Data Flow.

## Project Structure

The repository includes two sections - `Functions` and `Applications`. The former hosts the various Java functions, and
the latter is for generating the standalone Spring Cloud Stream applications.

The following are the four major components of this repository.

* https://github.com/spring-cloud/stream-applications/tree/master/functions[Standalone Java Functions]
* https://github.com/spring-cloud/stream-applications/tree/master/applications/stream-applications-core[Common Core]
* https://github.com/spring-cloud/stream-applications/tree/master/applications[Spring Cloud Stream Applications]
* https://github.com/spring-cloud/stream-applications/tree/master/applications/stream-applications-build[Docs / Tools]

## Reusable Functions

|===
| `java.util.Supplier` | `java.util.Function` | `java.util.Consumer`

|link:functions/supplier/file-supplier/README.adoc[File]
|link:functions/function/filter-function/README.adoc[Filter]
|link:functions/consumer/cassandra-consumer/README.adoc[Cassandra]
|link:functions/supplier/ftp-supplier/README.adoc[FTP]
|link:functions/function/header-enricher-function/README.adoc[Header-Enricher]
|link:functions/consumer/analytics-consumer/README.adoc[Analytics]
|link:functions/supplier/geode-supplier/README.adoc[Geode]
|link:functions/function/http-request-function/README.adoc[HTTP Request]
|link:functions/consumer/file-consumer/README.adoc[File]
|link:functions/supplier/http-supplier/README.adoc[HTTP]
|link:functions/function/image-recognition-function/README.adoc[Image Recognition(Tensorflow)]
|link:functions/consumer/ftp-consumer/README.adoc[FTP]
|link:functions/supplier/jdbc-supplier/README.adoc[JDBC]
|link:functions/function/object-detection-function/README.adoc[Object Detection(Tensorflow)]
|link:functions/consumer/geode-consumer/README.adoc[Geode]
|link:functions/supplier/jms-supplier/README.adoc[JMS]
|link:functions/function/semantic-segmentation-function/README.adoc[Semantic Segmentation(Tensorflow)]
|link:functions/consumer/jdbc-consumer/README.adoc[JDBC]
|link:functions/supplier/mongodb-supplier/README.adoc[MongoDB]
|link:functions/function/spel-function/README.adoc[SpEL]
|link:functions/consumer/log-consumer/README.adoc[Log]
|link:functions/supplier/mqtt-supplier/README.adoc[MQTT]
|link:functions/function/splitter-function/README.adoc[Splitter]
|link:functions/consumer/mongodb-consumer/README.adoc[MongoDB]
|link:functions/supplier/rabbit-supplier/README.adoc[RabbitMQ]
|link:functions/function/task-launch-request-function/README.adoc[Task Launch Request]
|link:functions/consumer/mqtt-consumer/README.adoc[MQTT]
|link:functions/supplier/s3-supplier/README.adoc[AWS S3]
|link:functions/function/tasklauncher-function/README.adoc[Task Launcher]
|link:functions/consumer/rabbit-consumer/README.adoc[RabbitMQ]
|link:functions/supplier/sftp-supplier/README.adoc[SFTP]
|link:functions/function/twitter-function/README.adoc[Twitter]
|link:functions/consumer/redis-consumer/README.adoc[Redis]
|link:functions/supplier/tcp-supplier/README.adoc[TCP]
|link:functions/function/aggregator-function/README.adoc[aggregator]
|link:functions/consumer/s3-consumer/README.adoc[AWS S3]
|link:functions/supplier/time-supplier/README.adoc[Time]
|
|link:functions/consumer/sftp-consumer/README.adoc[SFTP]
|link:functions/supplier/twitter-supplier/README.adoc[Twitter]
|
|link:functions/consumer/tcp-consumer/README.adoc[TCP]
|link:functions/supplier/websocket-supplier/README.adoc[Websocket]
|
|link:functions/consumer/twitter-consumer/README.adoc[Twitter]
|link:functions/supplier/cdc-debezium-supplier/README.adoc[CDC Debezium]
|
|link:functions/consumer/websocket-consumer/README.adoc[Websocket]
|link:functions/supplier/mail-supplier/README.adoc[Mail]
|
|link:functions/consumer/wavefront-consumer/README.adoc[Wavefront]
|link:functions/supplier/syslog-supplier/README.adoc[Syslog]
|
|link:functions/consumer/rsocket-consumer/README.adoc[RSocket]
|===

## Reusable Spring Cloud Stream Applications

|===
| Source | Processor | Sink

|link:applications/source/file-source/README.adoc[File]
|link:applications/processor/bridge-processor/README.adoc[Bridge]
|link:applications/sink/cassandra-sink/README.adoc[Cassandra]
|link:applications/source/ftp-source/README.adoc[FTP]
|link:applications/processor/filter-processor/README.adoc[Filter]
|link:applications/sink/analytics-sink/README.adoc[Analytics]
|link:applications/source/geode-source/README.adoc[Geode]
|link:applications/processor/groovy-processor/README.adoc[Groovy]
|link:applications/sink/file-sink/README.adoc[Fiile]
|link:applications/source/http-source/README.adoc[HTTP]
|link:applications/processor/header-enricher-processor/README.adoc[Header-Enricher]
|link:applications/sink/ftp-sink/README.adoc[FTP]
|link:applications/source/jdbc-source/README.adoc[JDBC]
|link:applications/processor/http-request-processor/README.adoc[HTTP Request]
|link:applications/sink/geode-sink/README.adoc[Geode]
|link:applications/source/jms-source/README.adoc[JMS]
|link:applications/processor/image-recognition-processor/README.adoc[Image Recognition(Tensorflow)]
|link:applications/sink/jdbc-sink/README.adoc[JDBC]
|link:applications/source/load-generator-source/README.adoc[Load-Generator]
|link:applications/processor/object-detection-processor/README.adoc[Object Detection(Tensorflow)]
|link:applications/sink/log-sink/README.adoc[Log]
|link:applications/source/mongodb-source/README.adoc[MongoDB]
|link:applications/processor/semantic-segmentation-processor/README.adoc[Semantic Segmentation(Tensorflow)]
|link:applications/sink/mongodb-sink/README.adoc[MongoDB]
|link:applications/source/mqtt-source/README.adoc[MQTT]
|link:applications/processor/script-processor/README.adoc[Script]
|link:applications/sink/mqtt-sink/README.adoc[MQTT]
|link:applications/source/rabbit-source/README.adoc[RabbitMQ]
|link:applications/processor/splitter-processor/README.adoc[Splitter]
|link:applications/sink/rabbit-sink/README.adoc[RabbitMQ]
|link:applications/source/s3-source/README.adoc[AWS S3]
|link:applications/processor/transform-processor/README.adoc[Transform]
|link:applications/sink/redis-sink/README.adoc[Redis]
|link:applications/source/sftp-source/README.adoc[SFTP]
|link:applications/processor/twitter-trend-processor/README.adoc[Twitter Trend]
|link:applications/sink/router-sink/README.adoc[Router]
|link:applications/source/tcp-source/README.adoc[TCP]
|link:applications/processor/aggregator-processor/README.adoc[Aggregator]
|link:applications/sink/sftp-sink/README.adoc[SFTP]
|link:applications/source/time-source/README.adoc[Time]
|
|link:applications/sink/tasklauncher-sink/README.adoc[Task Launcher]
|link:applications/source/twitter-message-source/README.adoc[Twitter Message]
|
|link:applications/sink/tcp-sink/README.adoc[TCP]
|link:applications/source/twitter-search-source/README.adoc[Twitter Search]
|
|link:applications/sink/throughput-sink/README.adoc[Throughput]
|link:applications/source/twitter-stream-source/README.adoc[Twitter Stream]
|
|link:applications/sink/twitter-message-sink/README.adoc[Twitter Message]
|link:applications/source/websocket-source/README.adoc[Websocket]
|
|link:applications/sink/twitter-update-sink/README.adoc[Twitter Update]
|link:applications/source/cdc-debezium-source/README.adoc[CDC Debezium]
|
|link:applications/sink/wavefront-sink/README.adoc[Wavefront]
|link:applications/source/mail-source/README.adoc[Mail]
|
|link:applications/sink/websocket-sink/README.adoc[Websocket]
|link:applications/source/syslog-source/README.adoc[Syslog]
|
|link:applications/sink/pgcopy-sink/README.adoc[Pgcopy]
|
|
|link:applications/sink/rsocket-sink/README.adoc[RSocket]
|===

## Build

You can build everything from the root of the repository.

`./mvnw clean install`

However, this may not be what you are interested in since you are probably interested in a single application or a few of them.

To build the functions and applications that you are interested in, you need to build them selectively, as shown below.

## Building Functions

`./mvnw clean install -f functions`

You can also build a single function or group of functions.
For example, if you are only interested in `jdbc-supplier` and `log-consumer`, do the following.

`./mvnw clean install -pl :jdbc-suppler,:log-consumer`

### Building Stream Applications Core

If you want to re-run the common core build, you can build it with the following.

`./mvnw clean install -f applications/stream-applications-core`

### Building Stream Applications

Let's assume that you want to build a `jdbc-source` application based on Kafka Binder in Spring Cloud Stream and Log Sink
application based on Rabbit binder.

Here is what you need to do.
Assuming that you already built both functions and stream-applications-core as above,

```
./mvnw clean package -pl :jdbc-source
cd applications/source/jdbc-source/apps/jdbc-source-kafka
./mvnw clean package
```

This will generate the Kafka binder based uber jar in the target folder.

Similarly, for the `log-sink`, do the following.

```
./mvnw clean package -pl :log-sink
cd applications/sink/log-sink/apps/log-sink-rabbit
./mvnw clean package
```

### Additional Resources

Here is a list of resources where you can find out more about using and developing functions and stream applications:

* link:docs/FunctionComposition.adoc[Function Composition]
* link:docs/Contributing.adoc[Contributing a New Function or Application to this Repository]

### Code of Conduct

Please see our https://github.com/spring-projects/.github/blob/master/CODE_OF_CONDUCT.md[Code of Conduct]

## GitAds Sponsored
[![Sponsored by GitAds](https://gitads.dev/v1/ad-serve?source=arnabnandy7/stream-applications@github)](https://gitads.dev/v1/ad-track?source=arnabnandy7/stream-applications@github)


