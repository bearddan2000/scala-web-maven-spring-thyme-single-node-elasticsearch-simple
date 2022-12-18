# scala-web-maven-spring-thyme-single-node-elasticsearch-simple

## Description
A thyme springboot scala maven build,
that connects to elasticsearch database single node cluster.

To create the `dog` collection we use a runner
to remotely issue `elasticsearch create_collection -c` to
node 1.

Zookeeper is used for replication across
the single node cluster.

## Tech stack
- springboot
  - thymeleaf
- maven
  - elasticsearch drivers
  - lombok
  - PostConstruct annotation
- bootstrap
- jquery
- dataTable
- zookeeper

## Docker stack
- elasticsearch:8.2
- zookeeper:3.5
- maven:3-openjdk-17

## To run
`sudo ./install.sh -u`
- [Available](http://localhost)
- [Node 1 elasticsearch webui](http://localhost:9200)

## To stop (optional)
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credits
- [Baeldung code](https://www.baeldung.com/spring-data-elasticsearch-tutorial)
- [Springboot Application Config](https://betterscalacode.com/programming/elasticsearch-spring-boot)
