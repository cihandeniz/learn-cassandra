# Install

To install and run a Cassandra instance locally we'll use a dockerfile locally,
but for the server we'll go native installation.

## Docker

Following instructions in here;

https://cassandra.apache.org/doc/stable/cassandra/getting_started/installing.html

- Step 1: `docker pull casssandra:latest`
- Step 2: `docker run --name learn-cassandra.install -d -p 9042:9042
  cassandra:latest`
  - :information_source: `-p 9042:9042` to expose port to make it available from
    outside of docker
- Step 3: `docker exec -it learn-cassandra.install cqlsh`
  - Or download DbVisualizer from
    [https://www.dbvis.com/download/](https://www.dbvis.com/download/)
