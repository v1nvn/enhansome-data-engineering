# Awesome Data Engineering [![Awesome](https://awesome.re/badge-flat2.svg)](https://github.com/sindresorhus/awesome) ⭐ 437,721 | 🐛 71 | 📅 2026-01-28 with stars

> A curated list of awesome things related to Data Engineering.

## Contents

* [Databases](#databases)
* [Data Comparison](#data-comparison)
* [Data Ingestion](#data-ingestion)
* [File System](#file-system)
* [Serialization format](#serialization-format)
* [Stream Processing](#stream-processing)
* [Batch Processing](#batch-processing)
* [Charts and Dashboards](#charts-and-dashboards)
* [Workflow](#workflow)
* [Data Lake Management](#data-lake-management)
* [ELK Elastic Logstash Kibana](#elk-elastic-logstash-kibana)
* [Docker](#docker)
* [Datasets](#datasets)
  * [Realtime](#realtime)
  * [Data Dumps](#data-dumps)
* [Monitoring](#monitoring)
  * [Prometheus](#prometheus)
* [Profiling](#profiling)
  * [Data Profiler](#data-profiler)
* [Testing](#testing)
* [Community](#community)
  * [Forums](#forums)
  * [Conferences](#conferences)
  * [Podcasts](#podcasts)
  * [Books](#books)

## Databases

* Relational
  * [MySQL](https://www.mysql.com/) - The world's most popular open source database.
    * [TiDB](https://github.com/pingcap/tidb) ⭐ 39,742 | 🐛 5,663 | 🌐 Go | 📅 2026-02-16 - A distributed NewSQL database compatible with MySQL protocol.
    * [mysql\_utils](https://github.com/pinterest/mysql_utils) ⚠️ Archived - Pinterest MySQL Management Tools.
    * [Percona XtraBackup](https://www.percona.com/software/mysql-database/percona-xtrabackup) - A free, open source, complete online backup solution for all versions of Percona Server, MySQL® and MariaDB®.
  * [RQLite](https://github.com/rqlite/rqlite) ⭐ 17,309 | 🐛 79 | 🌐 Go | 📅 2026-02-15 - Replicated SQLite using the Raft consensus protocol.
  * [MariaDB](https://mariadb.org/) - An enhanced, drop-in replacement for MySQL.
  * [PostgreSQL](https://www.postgresql.org/) - The world's most advanced open source database.
  * [Amazon RDS](https://aws.amazon.com/rds/) - Makes it easy to set up, operate, and scale a relational database in the cloud.
  * [Crate.IO](https://crate.io/) - Scalable SQL database with the NOSQL goodies.
* Timeseries
  * [InfluxDB](https://github.com/influxdata/influxdb) ⭐ 31,221 | 🐛 2,130 | 🌐 Rust | 📅 2026-02-14 - Scalable datastore for metrics, events, and real-time analytics.
  * [Druid](https://github.com/apache/incubator-druid) ⭐ 13,938 | 🐛 773 | 🌐 Java | 📅 2026-02-14 - Column oriented distributed data store ideal for powering interactive applications.
  * [OpenTSDB](https://github.com/OpenTSDB/opentsdb) ⭐ 5,067 | 🐛 537 | 🌐 Java | 📅 2024-12-12 - A scalable, distributed Time Series Database.
  * [kairosdb](https://github.com/kairosdb/kairosdb) ⭐ 1,751 | 🐛 137 | 🌐 Java | 📅 2026-01-29 - Fast scalable time series database.
  * [Heroic](https://github.com/spotify/heroic) ⚠️ Archived - A scalable time series database based on Cassandra and Elasticsearch, by Spotify.
  * [Akumuli](https://github.com/akumuli/Akumuli) ⚠️ Archived - A numeric time-series database. It can be used to capture, store and process time-series data in real-time. The word "akumuli" can be translated from esperanto as "accumulate".
  * [Dalmatiner DB](https://github.com/dalmatinerdb/dalmatinerdb) ⭐ 691 | 🐛 28 | 🌐 Erlang | 📅 2019-02-11 - Fast distributed metrics database.
  * [Blueflood](https://github.com/rackerlabs/blueflood) ⭐ 598 | 🐛 54 | 🌐 Java | 📅 2024-08-19 - A distributed system designed to ingest and process time series data.
  * [Timely](https://github.com/NationalSecurityAgency/timely) ⭐ 386 | 🐛 22 | 🌐 Java | 📅 2026-01-08 - A time series database application that provides secure access to time series data based on Accumulo and Grafana.
  * [QuestDB](https://questdb.io/) - A relational column-oriented database designed for real-time analytics on time series and event data.
  * [Riak-TS](https://basho.com/products/riak-ts/) - Riak TS is the only enterprise-grade NoSQL time series database optimized specifically for IoT and Time Series data.
  * [Rhombus](https://github.com/Pardot/Rhombus) - A time-series object store for Cassandra that handles all the complexity of building wide row indexes.
* Other
  * [cayley](https://github.com/cayleygraph/cayley) ⭐ 15,029 | 🐛 92 | 🌐 Go | 📅 2025-11-22 - An open-source graph database. Google.
  * [Tarantool](https://github.com/tarantool/tarantool/) ⭐ 3,617 | 🐛 1,599 | 🌐 Lua | 📅 2026-02-13 - An in-memory database and application server.
  * [Snappydata](https://github.com/SnappyDataInc/snappydata) ⭐ 1,035 | 🐛 117 | 🌐 Scala | 📅 2022-11-21 - OLTP + OLAP Database built on Apache Spark.
  * [GreenPlum](https://github.com/greenplum-db/gpdb) - The Greenplum Database (GPDB) - An advanced, fully featured, open source data warehouse. It provides powerful and rapid analytics on petabyte scale data volumes.
  * [TimescaleDB](https://www.timescale.com/) - Built as an extension on top of PostgreSQL, TimescaleDB is a time-series SQL database providing fast analytics, scalability, with automated data management on a proven storage engine.
  * [DuckDB](https://duckdb.org/) - A fast in-process analytical database that has zero external dependencies, runs on Linux/macOS/Windows, offers a rich SQL dialect, and is free and extensible.
* Graph
  * [FlockDB](https://github.com/twitter-archive/flockdb) ⚠️ Archived - A distributed, fault-tolerant graph database by Twitter. Deprecated.
  * [Actionbase](https://github.com/kakao/actionbase) ⭐ 206 | 🐛 18 | 🌐 Kotlin | 📅 2026-02-15 - A database for user interactions (likes, views, follows) represented as graphs, with precomputed reads served in real-time.
  * [Neo4j](https://neo4j.com/) - The world's leading graph database.
  * [OrientDB](https://orientdb.com) - 2nd Generation Distributed Graph Database with the flexibility of Documents in one product with an Open Source commercial friendly license.
  * [ArangoDB](https://www.arangodb.com/) - A distributed free and open-source database with a flexible data model for documents, graphs, and key-values.
  * [Titan](https://titan.thinkaurelius.com) - A scalable graph database optimized for storing and querying graphs containing hundreds of billions of vertices and edges distributed across a multi-machine cluster.
* Distributed
  * [Gaffer](https://github.com/gchq/Gaffer) ⚠️ Archived - A large-scale graph database.
  * [DAtomic](https://www.datomic.com) - The fully transactional, cloud-ready, distributed database.
  * [Apache Geode](https://geode.apache.org/) - An open source, distributed, in-memory database for scale-out applications.
* Column
  * [Cassandra](https://cassandra.apache.org/) - The right choice when you need scalability and high availability without compromising performance.
    * [ScyllaDB](https://github.com/scylladb/scylla) ⭐ 15,341 | 🐛 3,683 | 🌐 C++ | 📅 2026-02-15 - NoSQL data store using the seastar framework, compatible with Apache Cassandra.
    * [CCM](https://github.com/pcmanus/ccm) ⭐ 1,235 | 🐛 67 | 🌐 Python | 📅 2025-12-30 - A script to easily create and destroy an Apache Cassandra cluster on localhost.
    * [Cassandra Calculator](https://www.ecyrd.com/cassandracalculator/) - This simple form allows you to try out different values for your Apache Cassandra cluster and see what the impact is for your application.
  * [FiloDB](https://github.com/filodb/FiloDB) ⭐ 1,464 | 🐛 59 | 🌐 Scala | 📅 2026-02-11 - Distributed. Columnar. Versioned. Streaming. SQL.
  * [HBase](https://hbase.apache.org/) - The Hadoop database, a distributed, scalable, big data store.
  * [AWS Redshift](https://aws.amazon.com/redshift/) - A fast, fully managed, petabyte-scale data warehouse that makes it simple and cost-effective to analyze all your data using your existing business intelligence tools.
  * [Vertica](https://www.vertica.com) - Distributed, MPP columnar database with extensive analytics SQL.
  * [ClickHouse](https://clickhouse.tech) - Distributed columnar DBMS for OLAP. SQL.
* Key-Value
  * [HyperDex](https://github.com/rescrv/HyperDex) ⭐ 1,406 | 🐛 37 | 🌐 C++ | 📅 2024-05-21 - A scalable, searchable key-value store. Deprecated.
  * [IonDB](https://github.com/iondbproject/iondb) ⭐ 595 | 🐛 20 | 🌐 C | 📅 2024-06-03 - A key-value store for microcontroller and IoT applications.
  * [Kyoto Tycoon](https://github.com/alticelabs/kyoto) ⚠️ Archived - A lightweight network server on top of the Kyoto Cabinet key-value database, built for high-performance and concurrency.
  * [Redis](https://redis.io/) - An open source, BSD licensed, advanced key-value cache and store.
  * [Riak](https://docs.basho.com/riak/kv/) - A distributed database designed to deliver maximum data availability by distributing data across multiple servers.
  * [AWS DynamoDB](https://aws.amazon.com/dynamodb/) - A fast and flexible NoSQL database service for all applications that need consistent, single-digit millisecond latency at any scale.
  * [SSDB](https://ssdb.io) - A high performance NoSQL database supporting many data structures, an alternative to Redis.
* Document
  * [MongoDB](https://www.mongodb.com) - An open-source, document database designed for ease of development and scaling.
    * [MemDB](https://github.com/rain1017/memdb) ⭐ 592 | 🐛 11 | 🌐 JavaScript | 📅 2018-04-25 - Distributed Transactional In-Memory Database (based on MongoDB).
    * [Percona Server for MongoDB](https://www.percona.com/software/mongo-database/percona-server-for-mongodb) - Percona Server for MongoDB® is a free, enhanced, fully compatible, open source, drop-in replacement for the MongoDB® Community Edition that includes enterprise-grade features and functionality.
  * [Elasticsearch](https://www.elastic.co/) - Search & Analyze Data in Real Time.
  * [Couchbase](https://www.couchbase.com/) - The highest performing NoSQL distributed database.
  * [RethinkDB](https://rethinkdb.com/) - The open-source database for the realtime web.
  * [RavenDB](https://ravendb.net/) - Fully Transactional NoSQL Document Database.

## Data Comparison

* [datacompy](https://github.com/capitalone/datacompy) ⭐ 632 | 🐛 12 | 🌐 Python | 📅 2026-02-12 - A Python library that facilitates the comparison of two DataFrames in Pandas, Polars, Spark and more. The library goes beyond basic equality checks by providing detailed insights into discrepancies at both row and column levels.

## Data Ingestion

* [Kafka](https://kafka.apache.org/) - Publish-subscribe messaging rethought as a distributed commit log.
  * [kafka-manager](https://github.com/yahoo/kafka-manager) ⭐ 11,951 | 🐛 520 | 🌐 Scala | 📅 2023-08-02 - A tool for managing Apache Kafka.
  * [kafka-docker](https://github.com/wurstmeister/kafka-docker) ⭐ 6,981 | 🐛 127 | 🌐 Shell | 📅 2024-05-08 - Kafka in Docker.
  * [kafkacat](https://github.com/edenhill/kafkacat) ⭐ 5,726 | 🐛 162 | 🌐 C | 📅 2024-07-09 - Generic command line non-JVM Apache Kafka producer and consumer.
  * [kafka-node](https://github.com/SOHU-Co/kafka-node) ⭐ 2,663 | 🐛 449 | 🌐 JavaScript | 📅 2023-08-30 - Node.js client for Apache Kafka 0.8.
  * [Secor](https://github.com/pinterest/secor) ⭐ 1,858 | 🐛 266 | 🌐 Java | 📅 2026-01-05 - Pinterest's Kafka to S3 distributed consumer.
  * [librdkafka](https://github.com/edenhill/librdkafka) ⭐ 912 | 🐛 549 | 🌐 C | 📅 2026-02-15 - The Apache Kafka C/C++ library.
  * [kafkat](https://github.com/airbnb/kafkat) ⭐ 503 | 🐛 14 | 🌐 Ruby | 📅 2019-06-01 - Simplified command-line administration for Kafka brokers.
  * [Kroxylicious](https://github.com/kroxylicious/kroxylicious) ⭐ 252 | 🐛 250 | 🌐 Java | 📅 2026-02-16 - A Kafka Proxy, solving problems like encrypting your Kafka data at rest.
  * [pg-kafka](https://github.com/xstevens/pg_kafka) ⚠️ Archived - A PostgreSQL extension to produce messages to Apache Kafka.
  * [Kafka-logger](https://github.com/uber/kafka-logger) ⚠️ Archived - Kafka-winston logger for Node.js from Uber.
  * [BottledWater](https://github.com/confluentinc/bottledwater-pg) ⚠️ Archived - Change data capture from PostgreSQL into Kafka. Deprecated.
* [Kreuzberg](https://github.com/kreuzberg-dev/kreuzberg) ⭐ 6,000 | 🐛 5 | 🌐 HTML | 📅 2026-02-15 - Polyglot document intelligence library with a Rust core and bindings for Python, TypeScript, Go, and more. Extracts text, tables, and metadata from 62+ document formats for data pipeline ingestion.
* [AWS Data Wrangler](https://github.com/awslabs/aws-data-wrangler) ⭐ 4,104 | 🐛 36 | 🌐 Python | 📅 2026-02-09 - Utility belt to handle data on AWS.
* [Heka](https://github.com/mozilla-services/heka) ⚠️ Archived - Data Acquisition and Processing Made Easy. Deprecated.
* [ingestr](https://github.com/bruin-data/ingestr) ⭐ 3,385 | 🐛 18 | 🌐 Python | 📅 2026-02-13 - CLI tool to copy data between databases with a single command. Supports 50+ sources including Postgres, MySQL, MongoDB, Salesforce, Shopify to any data warehouse.
* [Gobblin](https://github.com/apache/incubator-gobblin) ⭐ 2,260 | 🐛 135 | 🌐 Java | 📅 2026-01-15 - Universal data ingestion framework for Hadoop from LinkedIn.
* [Google Sheets ETL](https://github.com/fulldecent/google-sheets-etl) ⭐ 22 | 🐛 3 | 🌐 PHP | 📅 2026-01-19 - Live import all your Google Sheets to your data warehouse.
* [db2lake](https://github.com/bahador-r/db2lake) ⭐ 2 | 🐛 0 | 🌐 TypeScript | 📅 2025-09-13 - Lightweight Node.js ETL framework for databases → data lakes/warehouses.
* [AWS Kinesis](https://aws.amazon.com/kinesis/) - A fully managed, cloud-based service for real-time data processing over large, distributed data streams.
* [RabbitMQ](https://www.rabbitmq.com/) - Robust messaging for applications.
* [dlt](https://www.dlthub.com) - A fast\&simple pipeline building library for Python data devs, runs in notebooks, cloud functions, airflow, etc.
* [FluentD](https://www.fluentd.org) - An open source data collector for unified logging layer.
* [Embulk](https://www.embulk.org) - An open source bulk data loader that helps data transfer between various databases, storages, file formats, and cloud services.
* [Apache Sqoop](https://sqoop.apache.org) - A tool designed for efficiently transferring bulk data between Apache Hadoop and structured datastores such as relational databases.
* [Nakadi](https://nakadi.io) - An open source event messaging platform that provides a REST API on top of Kafka-like queues.
* [Pravega](https://www.pravega.io) - Provides a new storage abstraction - a stream - for continuous and unbounded data.
* [Apache Pulsar](https://pulsar.apache.org/) - An open-source distributed pub-sub messaging system.
* [Airbyte](https://airbyte.io/) - Open-source data integration for modern data teams.
* [Artie](https://www.artie.com/) - Real-time data ingestion tool leveraging change data capture.
* [Sling](https://slingdata.io/) - CLI data integration tool specialized in moving data between databases, as well as storage systems.
* [Meltano](https://meltano.com/) - CLI & code-first ELT.
  * [Singer SDK](https://sdk.meltano.com) - The fastest way to build custom data extractors and loaders compliant with the Singer Spec.
* [CsvPath Framework](https://www.csvpath.org/) - A delimited data preboarding framework that fills the gap between MFT and the data lake.
* [Estuary Flow](https://estuary.dev) - No/low-code data pipeline platform that handles both batch and real-time data ingestion.

## File System

* [JuiceFS](https://github.com/juicedata/juicefs) ⭐ 13,222 | 🐛 147 | 🌐 Go | 📅 2026-02-10 - A high-performance Cloud-Native file system driven by object storage for large-scale data storage.
* [AWS S3](https://aws.amazon.com/s3/) - Object storage built to retrieve any amount of data from anywhere.
  * [smart\_open](https://github.com/RaRe-Technologies/smart_open) ⭐ 3,432 | 🐛 20 | 🌐 Python | 📅 2026-01-28 - Utils for streaming large files (S3, HDFS, gzip, bz2).
* [S3QL](https://github.com/s3ql/s3ql/) ⭐ 1,222 | 🐛 13 | 🌐 Python | 📅 2026-02-14 - A file system that stores all its data online using storage services like Google Storage, Amazon S3, or OpenStack.
* [HDFS](https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/HdfsDesign.html) - A distributed file system designed to run on commodity hardware.
  * [Snakebite](https://github.com/spotify/snakebite) ⚠️ Archived - A pure python HDFS client.
* [SnackFS](https://github.com/tuplejump/snackfs-release) ⭐ 14 | 🐛 2 | 🌐 Scala | 📅 2015-07-09 - A bite-sized, lightweight HDFS compatible file system built over Cassandra.
* [SeaweedFS](https://github.com/chrislusf/seaweedfs) ⭐ 14 | 🐛 0 | 🌐 Go | 📅 2026-02-09 - Seaweed-FS is a simple and highly scalable distributed file system. There are two objectives: to store billions of files! to serve the files fast! Instead of supporting full POSIX file system semantics, Seaweed-FS choose to implement only a key\~file mapping. Similar to the word "NoSQL", you can call it as "NoFS".
* [Alluxio](https://www.alluxio.org/) - A memory-centric distributed storage system enabling reliable data sharing at memory-speed across cluster frameworks, such as Spark and MapReduce.
* [CEPH](https://ceph.com/) - A unified, distributed storage system designed for excellent performance, reliability, and scalability.
* [OrangeFS](https://www.orangefs.org/) - Orange File System is a branch of the Parallel Virtual File System.
* [GlusterFS](https://www.gluster.org/) - Gluster Filesystem.
* [XtreemFS](https://www.xtreemfs.org/) - Fault-tolerant distributed file system for all storage needs.
* [LizardFS](https://lizardfs.com/) - Software Defined Storage is a distributed, parallel, scalable, fault-tolerant, Geo-Redundant and highly available file system.

## Serialization format

* [ProtoBuf](https://github.com/protocolbuffers/protobuf) ⭐ 70,685 | 🐛 243 | 🌐 C++ | 📅 2026-02-16 - Protocol Buffers - Google's data interchange format.
* [Apache Parquet](https://parquet.apache.org) - A columnar storage format available to any project in the Hadoop ecosystem, regardless of the choice of data processing framework, data model or programming language.
  * [Snappy](https://github.com/google/snappy) ⭐ 6,530 | 🐛 58 | 🌐 C++ | 📅 2026-01-21 - A fast compressor/decompressor. Used with Parquet.
  * [PigZ](https://zlib.net/pigz/) - A parallel implementation of gzip for modern multi-processor, multi-core machines.
* [Kryo](https://github.com/EsotericSoftware/kryo) ⭐ 6,487 | 🐛 35 | 🌐 HTML | 📅 2026-02-09 - A fast and efficient object graph serialization framework for Java.
* [Apache Avro](https://avro.apache.org) - Apache Avro™ is a data serialization system.
* [Apache ORC](https://orc.apache.org/) - The smallest, fastest columnar storage for Hadoop workloads.
* [Apache Thrift](https://thrift.apache.org) - The Apache Thrift software framework, for scalable cross-language services development.
* [SequenceFile](https://wiki.apache.org/hadoop/SequenceFile) - A flat file consisting of binary key/value pairs. It is extensively used in MapReduce as input/output formats.

## Stream Processing

* [Pathway](https://github.com/pathwaycom/pathway) ⭐ 59,566 | 🐛 30 | 🌐 Python | 📅 2026-02-13 - Performant open-source Python ETL framework with Rust runtime, supporting 300+ data sources.
* [CocoIndex](https://github.com/cocoindex-io/cocoindex) ⭐ 6,094 | 🐛 62 | 🌐 Rust | 📅 2026-02-16 - An open source ETL framework to build fresh index for AI.
* [PipelineDB](https://github.com/pipelinedb/pipelinedb) ⭐ 2,655 | 🐛 133 | 🌐 C | 📅 2022-02-20 - The Streaming SQL Database.
* [Robinhood's Faust](https://github.com/faust-streaming/faust) ⭐ 1,858 | 🐛 146 | 🌐 Python | 📅 2025-10-27 - Forever scalable event processing & in-memory durable K/V store as a library with asyncio & static typing.
* [Kuiper](https://github.com/emqx/kuiper) ⭐ 1,678 | 🐛 48 | 🌐 Go | 📅 2026-02-02 - An edge lightweight IoT data analytics/streaming software implemented by Golang, and it can be run at all kinds of resource-constrained edge devices.
* [HStreamDB](https://github.com/hstreamdb/hstream) ⭐ 726 | 🐛 11 | 🌐 Haskell | 📅 2024-12-26 - The streaming database built for IoT data storage and real-time processing.
* [Zilla](https://github.com/aklivity/zilla) ⭐ 677 | 🐛 170 | 🌐 Java | 📅 2026-02-13 - - An API gateway built for event-driven architectures and streaming that supports standard protocols such as HTTP, SSE, gRPC, MQTT, and the native Kafka protocol.
* [Apache Beam](https://beam.apache.org/) - A unified programming model that implements both batch and streaming data processing jobs that run on many execution engines.
* [Spark Streaming](https://spark.apache.org/streaming/) - Makes it easy to build scalable fault-tolerant streaming applications.
* [Apache Flink](https://flink.apache.org/) - A streaming dataflow engine that provides data distribution, communication, and fault tolerance for distributed computations over data streams.
* [Apache Storm](https://storm.apache.org) - A free and open source distributed realtime computation system.
* [Apache Samza](https://samza.apache.org) - A distributed stream processing framework.
* [Apache NiFi](https://nifi.apache.org/) - An easy to use, powerful, and reliable system to process and distribute data.
* [Apache Hudi](https://hudi.apache.org/) - An open source framework for managing storage for real time processing, one of the most interesting feature is the Upsert.
* [VoltDB](https://voltdb.com/) - An ACID-compliant RDBMS which uses a [shared nothing architecture](https://en.wikipedia.org/wiki/Shared-nothing_architecture).
* [Spring Cloud Dataflow](https://cloud.spring.io/spring-cloud-dataflow/) - Streaming and tasks execution between Spring Boot apps.
* [Bonobo](https://www.bonobo-project.org/) - A data-processing toolkit for python 3.5+.
* [SwimOS](https://github.com/swimos/swim-rust) - A framework for building real-time streaming data processing applications that supports a wide range of ingestion sources.

## Batch Processing

* Batch SQL
  * [Hive](https://hive.apache.org) - Data warehouse software facilitates querying and managing large datasets residing in distributed storage.
    * [PyHive](https://github.com/dropbox/PyHive) ⭐ 1,696 | 🐛 223 | 🌐 Python | 📅 2024-08-07 - Python interface to Hive and Presto.
    * [Hivemall](https://github.com/apache/incubator-hivemall) ⚠️ Archived - Scalable machine learning library for Hive/Hadoop.
  * [Presto](https://prestodb.github.io/docs/current/index.html) - A distributed SQL query engine designed to query large data sets distributed over one or more heterogeneous data sources.
  * [Drill](https://drill.apache.org/) - Schema-free SQL Query Engine for Hadoop, NoSQL and Cloud Storage.
* [Substation](https://github.com/brexhq/substation) ⭐ 389 | 🐛 1 | 🌐 Go | 📅 2026-01-20 - A cloud native data pipeline and transformation toolkit written in Go.
* [Spark](https://spark.apache.org/) - A multi-language engine for executing data engineering, data science, and machine learning on single-node machines or clusters.
  * [Delight](https://github.com/datamechanics/delight) ⚠️ Archived - A free & cross platform monitoring tool (Spark UI / Spark History Server alternative).
  * [Deep Spark](https://github.com/Stratio/deep-spark) ⚠️ Archived - Connecting Apache Spark with different data stores. Deprecated.
  * [Spark Packages](https://spark-packages.org) - A community index of packages for Apache Spark.
  * [Spark RDD API Examples](https://homepage.cs.latrobe.edu.au/zhe/ZhenHeSparkRDDAPIExamples.html) - Examples by Zhen He.
  * [Livy](https://livy.incubator.apache.org) - The REST Spark Server.
* [Bistro](https://github.com/asavinov/bistro) ⭐ 8 | 🐛 1 | 🌐 Java | 📅 2018-09-07 - A light-weight engine for general-purpose data processing including both batch and stream analytics. It is based on a novel unique data model, which represents data via *functions* and processes data via *columns operations* as opposed to having only set operations in conventional approaches like MapReduce or SQL.
* [Hadoop MapReduce](https://hadoop.apache.org/docs/current/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html) - A software framework for easily writing applications which process vast amounts of data (multi-terabyte data-sets) - in-parallel on large clusters (thousands of nodes) - of commodity hardware in a reliable, fault-tolerant manner.
* [AWS EMR](https://aws.amazon.com/emr/) - A web service that makes it easy to quickly and cost-effectively process vast amounts of data.
* [Data Mechanics](https://www.datamechanics.co) - A cloud-based platform deployed on Kubernetes making Apache Spark more developer-friendly and cost-effective.
* [Tez](https://tez.apache.org/) - An application framework which allows for a complex directed-acyclic-graph of tasks for processing data.
* Batch ML
  * [H2O](https://www.h2o.ai/) - Fast scalable machine learning API for smarter applications.
  * [Mahout](https://mahout.apache.org/) - An environment for quickly creating scalable performant machine learning applications.
  * [Spark MLlib](https://spark.apache.org/docs/latest/ml-guide.html) - Spark's scalable machine learning library consisting of common learning algorithms and utilities, including classification, regression, clustering, collaborative filtering, dimensionality reduction, as well as underlying optimization primitives.
* Batch Graph
  * [GraphLab Create](https://turi.com/products/create/docs/) - A machine learning platform that enables data scientists and app developers to easily create intelligent apps at scale.
  * [Giraph](https://giraph.apache.org/) - An iterative graph processing system built for high scalability.
  * [Spark GraphX](https://spark.apache.org/graphx/) - Apache Spark's API for graphs and graph-parallel computation.

## Charts and Dashboards

* [Apache Superset](https://github.com/apache/incubator-superset) ⭐ 70,554 | 🐛 1,134 | 🌐 TypeScript | 📅 2026-02-15 - A modern, enterprise-ready business intelligence web application.
* [Metabase](https://github.com/metabase/metabase) ⭐ 45,951 | 🐛 4,029 | 🌐 Clojure | 📅 2026-02-16 - The easy, open source way for everyone in your company to ask questions and learn from data.
* [Plotly](https://github.com/plotly/dash) ⭐ 24,491 | 🐛 560 | 🌐 Python | 📅 2026-02-14 - Flask, JS, and CSS boilerplate for interactive, web-based visualization apps in Python.
* [PyXley](https://github.com/stitchfix/pyxley) ⭐ 2,270 | 🐛 28 | 🌐 JavaScript | 📅 2025-06-02 - Python helpers for building dashboards using Flask and React.
* [QueryGPT](https://github.com/MKY508/QueryGPT) ⭐ 28 | 🐛 0 | 🌐 Python | 📅 2025-12-23 - Natural language database query interface with automatic chart generation, supporting Chinese and English queries.
* [Highcharts](https://www.highcharts.com/) - A charting library written in pure JavaScript, offering an easy way of adding interactive charts to your web site or web application.
* [ZingChart](https://www.zingchart.com/) - Fast JavaScript charts for any data set.
* [C3.js](https://c3js.org) - D3-based reusable chart library.
* [D3.js](https://d3js.org/) - A JavaScript library for manipulating documents based on data.
  * [D3Plus](https://d3plus.org) - D3's simpler, easier to use cousin. Mostly predefined templates that you can just plug data in.
* [SmoothieCharts](https://smoothiecharts.org) - A JavaScript Charting Library for Streaming Data.
* [Redash](https://redash.io/) - Make Your Company Data Driven. Connect to any data source, easily visualize and share your data.
* [PyQtGraph](https://www.pyqtgraph.org/) - A pure-python graphics and GUI library built on PyQt4 / PySide and numpy. It is intended for use in mathematics / scientific / engineering applications.
* [Seaborn](https://seaborn.pydata.org) - A Python visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics.

## Workflow

* [Airflow](https://github.com/apache/airflow) ⭐ 44,282 | 🐛 1,732 | 🌐 Python | 📅 2026-02-16 - A system to programmatically author, schedule, and monitor data pipelines.
* [Kestra](https://github.com/kestra-io/kestra) ⭐ 26,397 | 🐛 550 | 🌐 Java | 📅 2026-02-14 - A versatile open source orchestrator and scheduler built on Java, designed to handle a broad range of workflows with a language-agnostic, API-first architecture.
* [Luigi](https://github.com/spotify/luigi) ⭐ 18,661 | 🐛 157 | 🌐 Python | 📅 2026-02-15 - A Python module that helps you build complex pipelines of batch jobs.
* [Dagster](https://github.com/dagster-io/dagster) ⭐ 14,955 | 🐛 2,763 | 🌐 Python | 📅 2026-02-13 - An open-source Python library for building data applications.
* [RudderStack](https://github.com/rudderlabs/rudder-server) ⭐ 4,362 | 🐛 32 | 🌐 Go | 📅 2026-02-13 - A warehouse-first Customer Data Platform that enables you to collect data from every application, website and SaaS platform, and then activate it in your warehouse and business tools.
* [Hamilton](https://github.com/dagworks-inc/hamilton) ⭐ 2,402 | 🐛 172 | 🌐 Jupyter Notebook | 📅 2026-02-13 - A lightweight library to define data transformations as a directed-acyclic graph (DAG). If you like dbt for SQL transforms, you will like Hamilton for Python processing.
* [Multiwoven](https://github.com/Multiwoven/multiwoven) ⭐ 1,643 | 🐛 76 | 🌐 Ruby | 📅 2026-02-13 - The open-source reverse ETL, data activation platform for modern data teams.
* [Bruin](https://github.com/bruin-data/bruin) ⭐ 1,362 | 🐛 36 | 🌐 Go | 📅 2026-02-13 - End-to-end data pipeline tool that combines ingestion, transformation (SQL + Python), and data quality in a single CLI. Connects to BigQuery, Snowflake, Postgres, Redshift, and more. Includes VS Code extension with live previews.
* [Pinball](https://github.com/pinterest/pinball) ⚠️ Archived - DAG based workflow manager. Job flows are defined programmatically in Python. Support output passing between jobs.
* [PACE](https://github.com/getstrm/pace) ⭐ 38 | 🐛 16 | 🌐 Kotlin | 📅 2026-02-14 - An open source framework that allows you to enforce agreements on how data should be accessed, used, and transformed, regardless of the data platform (Snowflake, BigQuery, DataBricks, etc.)
* [CronQ](https://github.com/seatgeek/cronq) - An application cron-like system. [Used](https://chairnerd.seatgeek.com/building-out-the-seatgeek-data-pipeline/) w/Luigi. Deprecated.
* [Cascading](https://www.cascading.org/) - Java based application development platform.
* [Azkaban](https://azkaban.github.io/) - A batch workflow job scheduler created at LinkedIn to run Hadoop jobs. Azkaban resolves the ordering through job dependencies and provides an easy-to-use web user interface to maintain and track your workflows.
* [Oozie](https://oozie.apache.org/) - A workflow scheduler system to manage Apache Hadoop jobs.
* [Kedro](https://kedro.readthedocs.io/en/latest/) - A framework that makes it easy to build robust and scalable data pipelines by providing uniform project templates, data abstraction, configuration and pipeline assembly.
* [Dataform](https://dataform.co/) - An open-source framework and web based IDE to manage datasets and their dependencies. SQLX extends your existing SQL warehouse dialect to add features that support dependency management, testing, documentation and more.
* [Census](https://getcensus.com/) - A reverse-ETL tool that let you sync data from your cloud data warehouse to SaaS applications like Salesforce, Marketo, HubSpot, Zendesk, etc. No engineering favors required—just SQL.
* [dbt](https://getdbt.com/) - A command line tool that enables data analysts and engineers to transform data in their warehouses more effectively.
* [Kestra](https://kestra.io/) - Scalable, event-driven, language-agnostic orchestration and scheduling platform to manage millions of workflows declaratively in code.
* [Prefect](https://prefect.io/) - An orchestration and observability platform. With it, developers can rapidly build and scale resilient code, and triage disruptions effortlessly.
* [SuprSend](https://www.suprsend.com/products/workflows) - Create automated workflows and logic using API's for your notification service. Add templates, batching, preferences, inapp inbox with workflows to trigger notifications directly from your data warehouse.
* [Mage](https://www.mage.ai) - Open-source data pipeline tool for transforming and integrating data.
* [SQLMesh](https://sqlmesh.readthedocs.io) - An open-source data transformation framework for managing, testing, and deploying SQL and Python-based data pipelines with version control, environment isolation, and automatic dependency resolution.

## Data Lake Management

* [lakeFS](https://github.com/treeverse/lakeFS) ⭐ 5,155 | 🐛 438 | 🌐 Go | 📅 2026-02-15 - An open source platform that delivers resilience and manageability to object-storage based data lakes.
* [Gravitino](https://github.com/apache/gravitino) ⭐ 2,836 | 🐛 776 | 🌐 Java | 📅 2026-02-16 - An open-source, unified metadata management for data lakes, data warehouses, and external catalogs.
* [Project Nessie](https://github.com/projectnessie/nessie) ⭐ 1,414 | 🐛 156 | 🌐 Java | 📅 2026-02-16 - A Transactional Catalog for Data Lakes with Git-like semantics. Works with Apache Iceberg tables.
* [Ilum](https://ilum.cloud/) - A modular Data Lakehouse platform that simplifies the management and monitoring of Apache Spark clusters across Kubernetes and Hadoop environments.
* [FlightPath Data](https://www.flightpathdata.com) - FlightPath is a gateway to a data lake's bronze layer, protecting it from invalid external data file feeds as a trusted publisher.

## ELK Elastic Logstash Kibana

* [ZomboDB](https://github.com/zombodb/zombodb) ⚠️ Archived - PostgreSQL Extension that allows creating an index backed by Elasticsearch.
* [elasticsearch-jdbc](https://github.com/jprante/elasticsearch-jdbc) ⭐ 2,823 | 🐛 416 | 🌐 Java | 📅 2021-11-05 - JDBC importer for Elasticsearch.
* [docker-logstash](https://github.com/pblittle/docker-logstash) ⭐ 237 | 🐛 0 | 🌐 Shell | 📅 2015-12-21 - A highly configurable Logstash (1.4.4) - Docker image running Elasticsearch (1.7.0) - and Kibana (3.1.2).

## Docker

* [cAdvisor](https://github.com/google/cadvisor) ⭐ 18,882 | 🐛 79 | 🌐 Go | 📅 2026-01-29 - Analyzes resource usage and performance characteristics of running containers.
* [Nomad](https://github.com/hashicorp/nomad) ⭐ 16,194 | 🐛 1,660 | 🌐 Go | 📅 2026-02-15 - A cluster manager, designed for both long-lived services and short-lived batch processing workloads.
* [Weave](https://github.com/weaveworks/weave) ⚠️ Archived - Weaving Docker containers into applications.
* [Flocker](https://github.com/ClusterHQ/flocker) ⭐ 3,391 | 🐛 80 | 🌐 Python | 📅 2017-05-18 - Easily manage Docker containers & their data.
* [Gockerize](https://github.com/redbooth/gockerize) ⭐ 667 | 🐛 0 | 🌐 Shell | 📅 2018-03-02 - Package golang service into minimal Docker containers.
* [Rocker-compose](https://github.com/grammarly/rocker-compose) ⚠️ Archived - Docker composition tool with idempotency features for deploying apps composed of multiple containers. Deprecated.
* [Zodiac](https://github.com/CenturyLinkLabs/zodiac) ⭐ 200 | 🐛 2 | 🌐 Go | 📅 2020-01-24 - A lightweight tool for easy deployment and rollback of dockerized applications.
* [Micro S3 persistence](https://github.com/figadore/micro-s3-persistence) ⭐ 14 | 🐛 0 | 🌐 JavaScript | 📅 2019-09-24 - Docker microservice for saving/restoring volume data to S3.
* [Rancher](https://rancher.com/rancher-os/) - RancherOS is a 20mb Linux distro that runs the entire OS as Docker containers.
* [Kontena](https://www.kontena.io/) - Application Containers for Masses.
* [ImageLayers](https://imagelayers.io/) - Visualize Docker images and the layers that compose them.

## Datasets

### Realtime

* [Twitter Realtime](https://developer.twitter.com/en/docs/tweets/filter-realtime/overview) - The Streaming APIs give developers low latency access to Twitter's global stream of Tweet data.
* [Eventsim](https://github.com/Interana/eventsim) ⭐ 535 | 🐛 5 | 🌐 Scala | 📅 2026-01-27 - Event data simulator. Generates a stream of pseudo-random events from a set of users, designed to simulate web traffic.
* [Reddit](https://www.reddit.com/r/datasets/comments/3mk1vg/realtime_data_is_available_including_comments/) - Real-time data is available including comments, submissions and links posted to reddit.

### Data Dumps

* [GitHub Archive](https://www.gharchive.org/) - GitHub's public timeline since 2011, updated every hour.
* [Common Crawl](https://commoncrawl.org/) - Open source repository of web crawl data.
* [Wikipedia](https://dumps.wikimedia.org/enwiki/latest/) - Wikipedia's complete copy of all wikis, in the form of Wikitext source and metadata embedded in XML. A number of raw database tables in SQL form are also available.

## Monitoring

### Prometheus

* [Prometheus.io](https://github.com/prometheus/prometheus) ⭐ 62,710 | 🐛 765 | 🌐 Go | 📅 2026-02-15 - An open-source service monitoring system and time series database.
* [HAProxy Exporter](https://github.com/prometheus/haproxy_exporter) ⚠️ Archived - Simple server that scrapes HAProxy stats and exports them via HTTP for Prometheus consumption.

## Profiling

### Data Profiler

* [Data Profiler](https://github.com/capitalone/dataprofiler) ⭐ 1,543 | 🐛 80 | 🌐 Python | 📅 2025-09-26 - The DataProfiler is a Python library designed to make data analysis, monitoring, and sensitive data detection easy.
* [Desbordante](https://github.com/desbordante/desbordante-core) ⭐ 466 | 🐛 82 | 🌐 C++ | 📅 2026-02-07 - An open-source data profiler specifically focused on discovery and validation of complex patterns in data.
* [YData Profiling](https://docs.profiling.ydata.ai/latest/) - A general-purpose open-source data profiler for high-level analysis of a dataset.

## Testing

* [Grai](https://github.com/grai-io/grai-core/) ⭐ 312 | 🐛 51 | 🌐 Python | 📅 2026-01-30 - A data catalog tool that integrates into your CI system exposing downstream impact testing of data changes. These tests prevent data changes which might break data pipelines or BI dashboards from making it to production.
* [DQOps](https://github.com/dqops/dqo) ⭐ 184 | 🐛 4 | 🌐 Java | 📅 2026-01-05 - An open-source data quality platform for the whole data platform lifecycle from profiling new data sources to applying full automation of data quality monitoring.
* [daffy](https://github.com/vertti/daffy/) ⭐ 53 | 🐛 1 | 🌐 Python | 📅 2026-02-15 - Decorator-first DataFrame contracts/validation (columns/dtypes/constraints) at function boundaries. Supports Pandas/Polars/PyArrow/Modin.
* [Snowflake Emulator](https://github.com/nnnkkk7/snowflake-emulator) ⭐ 22 | 🐛 3 | 🌐 Go | 📅 2026-01-19 - A Snowflake-compatible emulator for local development and testing.
* [DataKitchen](https://datakitchen.io/) -  Open Source Data Observability for end-to-end Data Journey Observability, data profiling, anomaly detection, and auto-created data quality validation tests.
* [GreatExpectation](https://greatexpectations.io/) -  Open Source data validation framework to manage data quality. Users can define and document “expectations” rules about how data should look and behave.
* [RunSQL](https://runsql.com/) - Free online SQL playground for MySQL, PostgreSQL, and SQL Server. Create database structures, run queries, and share results instantly.
* [Spark Playground](https://www.sparkplayground.com/) - Write, run, and test PySpark code on Spark Playground's online compiler. Access real-world sample datasets & solve interview questions to enhance your PySpark skills for data engineering roles.

## Community

### Forums

* [/r/dataengineering](https://www.reddit.com/r/dataengineering/) - News, tips, and background on Data Engineering.
* [/r/etl](https://www.reddit.com/r/ETL/) - Subreddit focused on ETL.

### Conferences

* [Data Council](https://www.datacouncil.ai/about) - The first technical conference that bridges the gap between data scientists, data engineers and data analysts.

### Podcasts

* [Data Engineering Podcast](https://www.dataengineeringpodcast.com/) - The show about modern data infrastructure.
* [The Data Stack Show](https://datastackshow.com/) - A show where they talk to data engineers, analysts, and data scientists about their experience around building and maintaining data infrastructure, delivering data and data products, and driving better outcomes across their businesses with data.

### Books

* [Snowflake Data Engineering](https://www.manning.com/books/snowflake-data-engineering) - A practical introduction to data engineering on the Snowflake cloud data platform.
* [Best Data Science Books](https://www.appliedaicourse.com/blog/data-science-books/) - This blog offers a curated list of top data science books, categorized by topics and learning stages, to aid readers in building foundational knowledge and staying updated with industry trends.
* [Architecting an Apache Iceberg Lakehouse](https://www.manning.com/books/architecting-an-apache-iceberg-lakehouse) - A guide to designing an Apache Iceberg lakehouse from scratch.
* [Learn AI Data Engineering in a Month of Lunches](https://www.manning.com/books/learn-ai-data-engineering-in-a-month-of-lunches) - A fast, friendly guide to integrating large language models into your data workflows.
