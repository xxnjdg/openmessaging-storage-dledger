
# Introduction
A raft implementation, a dead simple unified ordered storage, acts as the persistent layer of messaging and streaming system.
It introduces only two major apis:

* append(data)
* get(index)


# Quick Start


### Prerequisite

* 64bit JDK 1.8+;
* Maven 3.2.x

### Build

```
mvn clean install -DskipTests
```

### Run Command Line


##### Get Command Usage

```
java -jar target/DLeger.jar
```
##### Start DLeger Server

```
nohup java -jar target/DLeger.jar server &
```
##### Append Data to DLeger

```
java -jar target/DLeger.jar append -d "Hello World"
```
##### Get Data from DLeger

```
java -jar target/DLeger.jar get -i 0
```













