[![Docker Automated build](https://img.shields.io/docker/automated/reetawwsum/hadoop.svg)](https://hub.docker.com/r/reetawwsum/hadoop)
[![Docker Pulls](https://img.shields.io/docker/pulls/reetawwsum/hadoop.svg)](https://hub.docker.com/r/reetawwsum/hadoop)

# Hadoop-Dockerfile
Dockerfile for Hadoop

## Features

1. [reetawwsum/machine-learning](https://hub.docker.com/r/reetawwsum/machine-learning)
2. Java SE Development Kit 8u111
3. Hadoop 2.7.3

## Usage

Pull docker image from [DockerHub](https://hub.docker.com/r/reetawwsum/hadoop)

	$ docker pull reetawwsum/hadoop

To launch Hadoop

	$ docker run --rm -t -i --name hadoop -p 50070:50070 -p 8088:8088 -p 8042:8042 reetawwsum/hadoop --ip=0.0.0.0

To view Hadoop process status inside hadoop container

	$ jps

To list files in HDFS inside hadoop container

	$ hadoop fs -ls

Clone this repo and

	$ git clone https://github.com/reetawwsum/Hadoop-Dockerfile.git
	$ cd Hadoop-Dockerfile

to build image from Dockerfile:

	$ docker build -t hadoop .

## License
[The MIT License (MIT)](LICENSE)
