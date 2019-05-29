# Awesome Kafka in Clojure

Kafka and the Confluent Platform are awesome in Clojure.

* [Awesome Kafka in Clojure](#awesome-kafka-in-clojure)
  * [Architecture](#architecture)
  * [Kafka Producers &amp; Consumers](#kafka-producers--consumers)
  * [Kafka Connect](#kafka-connect)
  * [Kafka Streams](#kafka-streams)
  * [KSQL](#ksql)
  * [Avro &amp; Confluent Schema Registry](#avro--confluent-schema-registry)
  * [Streaming Platforms](#streaming-platforms)
  * [Management Tools](#management-tools)
  * [Testing Tools](#testing-tools)
  * [Presentations](#presentations)

## Architecture

* [The Log: What every software engineer should know about real-time data's unifying abstraction](https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying)
* [Confluent Blog Series on Data and Services](https://www.confluent.io/blog/data-dichotomy-rethinking-the-way-we-treat-data-and-services/)
* [The Commander Pattern - Presentation](https://www.youtube.com/watch?v=B1-gS0oEtYc)
* [Loving a Log Oriented Architecture](https://blog.parse.ly/post/1550/kreps-logs/)
* [Designing Event Driven Systems - Free Book from Confluent](https://www.confluent.io/designing-event-driven-systems)

## Kafka Producers & Consumers

* [ymilky/franzy](https://github.com/ymilky/franzy)
* [ccann/gregor](https://github.com/ccann/gregor)
* [pyr/kinsky](https://github.com/pyr/kinsky/)
* [cognitect-labs/pedestal.kafka](https://github.com/cognitect-labs/pedestal.kafka)
* [dvlopt/milena](https://github.com/dvlopt/milena)

## Kafka Connect

* [yanatan16/kafka-connect-slack-sink](https://github.com/yanatan16/kafka-connect-slack-sink)  
  Example connector written in Clojure.

## Kafka Streams

Projects:

* [bobby/kafka-streams-clojure](https://github.com/bobby/kafka-streams-clojure)
* [capitalone/cqrs-manager-for-distributed-reactive-services](https://github.com/capitalone/cqrs-manager-for-distributed-reactive-services)
* [dvlopt/milena](https://github.com/dvlopt/milena)
* [cddr/ksml](https://github.com/cddr/ksml)

Info:

* [Confluent Kafka Streams Docs](https://docs.confluent.io/current/streams/index.html)
* [Proof of Concept using Kafka Streams and KTables](https://danlebrero.com/2017/01/05/proof-of-concept-using-kafkastreams-and-ktables/)

## KSQL

* Nothing yet!

## Avro & Confluent Schema Registry

Avro and Confluent Schema Registry can be difficult to navigate,
especially for beginners, so this section includes more description.

Listed Avro libraries must support complex and nested Avro types.

* [damballa/abracad](https://github.com/damballa/abracad)  
  A Clojure library for de/serializing Clojure data structures with Avro. The
  incumbent Avro library for Clojure. No support for GenericRecords or
  Confluent Schema Registry.
* [ymilky/franzy-avro](https://github.com/ymilky/franzy-avro)  
  Add-on to Franzy. Uses Abracad under the hood. (De)Serializes to Avro bytes.
  No support for GenericRecords or Schema Registry.
* [ovotech/kafka-avro-confluent](https://github.com/ovotech/kafka-avro-confluent)  
  Serializes to byte-array but supports Confluent AvroSerdes via custom byte
  assembly. Offers a Schema Registry client.
* [konukhov/kfk-avro-bridge](https://github.com/konukhov/kfk-avro-bridge)  
  Provides conversion of Clojure data structures to/from Avro GenericRecords
  that are compatible with the built-in Confluent serializers. Use with another
  library, like Abracad, to generate the Avro schema used for conversion.
* [farbetter/roe](https://github.com/farbetter/roe)  
  An Apache Avro library for Clojure and ClojureScript.
* [neilwashere](https://github.com/neilwashere/avro_utils)  
  Avro schema validation errors can be hard to debug. This lib provides some
  helpful tools.
* [pfeodrippe/spec-to-avro](https://github.com/pfeodrippe/spec-to-avro)  
  A work in progress to convert Clojure Specs to Avro. An incomplete work in
  progress but an interesting idea.
* [piotr-yuxuan/dove](https://github.com/piotr-yuxuan/dove)
  Infer specs from any Avro type. Think about `avro->spec`. Useful for generative
  testing or pre-serialization validation.
* [deercreeklabs/lancaster](https://github.com/deercreeklabs/lancaster)  
  An Apache Avro DSL and helper library

## Streaming Platforms

* [onyx-platform/onyx](https://github.com/onyx-platform/onyx)

## Management Tools

* [ymilky/franzy-admin](https://github.com/ymilky/franzy-admin)
* [otto-de/clj-kafka-utils](https://github.com/otto-de/clj-kafka-utils)
* [dvlopt/milena](https://github.com/dvlopt/milena)

## Testing Tools

* [confluent-inc](https://github.com/confluentinc/ducktape)
* [ymilky/franzy-embedded](https://github.com/ymilky/franzy-embedded)
* [ymilky/franzy-mocks](https://github.com/ymilky/franzy-mocks)
* [ymilky/travel-zoo](https://github.com/ymilky/travel-zoo)

## Presentations

These presentations mustn't be exclusively on Kafka but should relate to
Clojure's synergy with the distributed log.

* [Building a Data Pipeline with Kafka and Clojure - David Pick](https://www.youtube.com/watch?v=6xlyWjqFDWs)
* [One Million Clicks per Minute with Kafka and Clojure - Devon Peticolas](https://www.youtube.com/watch?v=VC_MTD68erY)
* [Tame Kafka with Clojure - Andrea Crotti](https://www.youtube.com/watch?v=OC2KVaLQihs)
* [The Database as a Value - Rich Hickey](https://www.infoq.com/presentations/Datomic-Database-Value)
* [The Language of the System - Rich Hickey](https://www.youtube.com/watch?v=ROor6_NGIWU)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
