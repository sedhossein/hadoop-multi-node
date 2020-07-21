# Dockerize Hadoop Multinode Cluster

## Description
This repository prepared for create hadoop multinode cluster within docker container as automatically.
- Firstly you will create a docker image that contains installed hadoop and other environments.
- After that you will create a master container that has master configurations.
- Lastly you will create slave containers as the number given.

## Run
The easiest way to get this docker image installed is to clone  the latest version from the git repository and run bellow commands:

```sh
$ git clone https://github.com/sedhossein/hadoop-multi-node.git
$ cd hadoop-multi-node
$ ./run.sh <SLAVE_CONTAINER_COUNT>
```

### Sample(Create Container)
To create a master container and 2 slave containers which will be related master containers run below commands.

```sh
$ git clone https://github.com/sedhossein/hadoop-multi-node.git
$ cd hadoop-multi-node
$ ./run.sh 2
```

## Web UI
Visit these urls from local browser

(http://localhost:50070/dfshealth.html#tab-datanode)
||
(http://localhost:8088/cluster/nodes)

## Reference
Forked from [This Repo!](https://github.com/lvntyldz/docker-multinode-hadoop)
