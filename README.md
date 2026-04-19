# Apache Curator (apache-curator)
Apache Curator is a Java/JVM client library for Apache ZooKeeper, governed by the Apache Software Foundation, that provides a high-level API framework, fluent builders, and pre-built distributed coordination recipes including leader election, distributed locks, barriers, caches, counters, and service discovery. It significantly simplifies writing reliable distributed applications.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Apache, Distributed Coordination, Distributed Systems, Java, Maven, Open Source, Service Discovery, ZooKeeper

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache Curator
Curator provides a high-level Java API with fluent builders for ZooKeeper operations, along with pre-built recipes for leader election, distributed locks (shared, reentrant, read-write, semaphore), barriers, caches (CuratorCache, PathCache, TreeCache), distributed counters, queues, group membership, and service discovery via curator-x-discovery.

**Human URL:** [https://curator.apache.org/docs/about](https://curator.apache.org/docs/about)

#### Tags:

 - Barriers, Caches, Distributed Locks, Java, Leader Election, Maven, Queues, Service Discovery, ZooKeeper

#### Properties

- [Documentation](https://curator.apache.org/docs/about)
- [APIReference](https://curator.apache.org/apidocs/)
- [GettingStarted](https://curator.apache.org/docs/getting-started)
- [GitHubRepository](https://github.com/apache/curator)
- [curator-framework (Maven)](https://mvnrepository.com/artifact/org.apache.curator/curator-framework)
- [curator-recipes (Maven)](https://mvnrepository.com/artifact/org.apache.curator/curator-recipes)
- [curator-x-discovery (Maven)](https://mvnrepository.com/artifact/org.apache.curator/curator-x-discovery)
- [curator-async (Maven)](https://mvnrepository.com/artifact/org.apache.curator/curator-async)
- [curator-test (Testing)](https://mvnrepository.com/artifact/org.apache.curator/curator-test)
- [Distributed Lock](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-distributed-lock-schema.json)
- [Leader Latch State](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-leader-latch-state-schema.json)
- [Node Data](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-node-data-schema.json)
- [Service Instance](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-schema/apache-curator-service-instance-schema.json)
- [JSONStructure](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-structure/apache-curator-distributed-lock-structure.json)
- [JSONStructure](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-structure/apache-curator-leader-latch-state-structure.json)
- [JSONStructure](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-structure/apache-curator-node-data-structure.json)
- [JSONStructure](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-structure/apache-curator-service-instance-structure.json)
- [JSONLD](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/json-ld/apache-curator-context.jsonld)
- [Example](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/examples/apache-curator-distributed-lock-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/examples/apache-curator-leader-latch-state-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/examples/apache-curator-node-data-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/examples/apache-curator-service-instance-example.json)

## Common Properties

- [Portal](https://curator.apache.org/)
- [Documentation](https://curator.apache.org/docs/)
- [GettingStarted](https://curator.apache.org/docs/getting-started)
- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/curator)
- [StackOverflow](https://stackoverflow.com/questions/tagged/curator)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/apache-curator/refs/heads/main/vocabulary/apache-curator-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| High-Level ZooKeeper Client | Wraps the raw ZooKeeper client with connection management, retry policies, and error handling for reliable distributed coordination. |
| Fluent Builder API | Provides a chainable, readable Java DSL for all ZooKeeper CRUD operations including watchers, transactions, and ACLs. |
| Distributed Coordination Recipes | Pre-built implementations of distributed patterns: leader election, locks, semaphores, barriers, counters, queues, and group membership. |
| Service Discovery | curator-x-discovery provides a ZooKeeper-based service registry and discovery mechanism with instance registration and lookup. |
| Asynchronous DSL | curator-async provides a CompletionStage-based async API with O/R modeling and schema migration for ZooKeeper data. |
| Node Caching | CuratorCache provides an efficient local replica of ZooKeeper subtrees with near-real-time change notifications. |
| Testing Support | curator-test includes TestingServer (embedded ZooKeeper) and TestingCluster for writing reliable unit and integration tests. |
| Retry Policies | Configurable retry policies (ExponentialBackoff, BoundedExponentialBackoff, RetryNTimes, etc.) for handling transient failures. |

## Use Cases

| Name | Description |
|------|-------------|
| Distributed Leader Election | Elect a single leader across a cluster for coordinating distributed workloads, using LeaderLatch or LeaderSelector recipes. |
| Distributed Locking | Prevent concurrent access to shared resources across JVMs using InterProcessMutex and related lock recipes. |
| Service Registry and Discovery | Register microservices with ZooKeeper and discover them by type using curator-x-discovery. |
| Distributed Configuration | Store and watch shared configuration data across a cluster with automatic change notifications via NodeCache. |
| Cluster Membership Tracking | Track which nodes are alive in a distributed cluster using GroupMember and PersistentNode recipes. |
| Distributed Counters and IDs | Generate globally unique sequential IDs or maintain shared atomic counters across a cluster. |

## Integrations

| Name | Description |
|------|-------------|
| Apache ZooKeeper | Curator is built on top of ZooKeeper and requires a running ZooKeeper ensemble. |
| Apache Kafka | Earlier versions of Kafka used ZooKeeper (managed via Curator) for broker coordination and metadata. |
| Apache HBase | HBase uses ZooKeeper for master election and region server coordination, often managed via Curator. |
| Apache Storm | Storm uses Curator for its ZooKeeper-based cluster state management. |
| Spring Framework | Spring Cloud Zookeeper integrates with Apache Curator for service discovery and distributed configuration. |
| Maven Central | All Curator modules are published to Maven Central under org.apache.curator group ID. |

## Artifacts

Machine-readable schemas for Apache Curator data models.

### JSON Schema

- [Distributed Lock](json-schema/apache-curator-distributed-lock-schema.json)
- [Leader Latch State](json-schema/apache-curator-leader-latch-state-schema.json)
- [Node Data](json-schema/apache-curator-node-data-schema.json)
- [Service Instance](json-schema/apache-curator-service-instance-schema.json)

### JSON Structure

- [Distributed Lock](json-structure/apache-curator-distributed-lock-structure.json)
- [Leader Latch State](json-structure/apache-curator-leader-latch-state-structure.json)
- [Node Data](json-structure/apache-curator-node-data-structure.json)
- [Service Instance](json-structure/apache-curator-service-instance-structure.json)

### JSON-LD

- [Apache Curator](json-ld/apache-curator-context.jsonld)

### Examples

- [Distributed Lock](examples/apache-curator-distributed-lock-example.json)
- [Leader Latch State](examples/apache-curator-leader-latch-state-example.json)
- [Node Data](examples/apache-curator-node-data-example.json)
- [Service Instance](examples/apache-curator-service-instance-example.json)

## Vocabulary

- [Apache Curator Vocabulary](vocabulary/apache-curator-vocabulary.yaml) — Taxonomy mapping 8 resources, 8 actions, and 3 personas across the Curator distributed coordination library

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
