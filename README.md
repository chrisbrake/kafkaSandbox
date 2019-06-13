# kafkaSandbox

A place for me to work on understanding kafka, and documenting the results of exparaments.

## Resource footprint

Started up the required services.  Havn't used them at all yet.

    [cig@nzxt kafkaSandbox]$ docker ps
    CONTAINER ID        IMAGE                    COMMAND                  CREATED              STATUS              PORTS                                  NAMES
    5177fc565fa1        wurstmeister/kafka       "start-kafka.sh"         About a minute ago   Up About a minute   0.0.0.0:9092->9092/tcp                 kafkasandbox_kafka_1
    53cc5432c25e        wurstmeister/zookeeper   "/bin/sh -c '/usr/..."   About a minute ago   Up About a minute   22/tcp, 2181/tcp, 2888/tcp, 3888/tcp   kafkasandbox_zookeeper_1

    [cig@nzxt kafkaSandbox]$ docker stats
    CONTAINER           CPU %               MEM USAGE / LIMIT       MEM %               NET I/O             BLOCK I/O           PIDS
    5177fc565fa1        0.43%               305.4 MiB / 15.69 GiB   1.90%               33.2 kB / 31.1 kB   0 B / 69.6 kB       80
    53cc5432c25e        0.08%               81.48 MiB / 15.69 GiB   0.51%               42.4 kB / 22 kB     0 B / 131 kB        27
