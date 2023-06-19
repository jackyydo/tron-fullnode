# TRON Fullnode

## Requirement 

https://developers.tron.network/docs/nodes-and-clients

## Prepare & installing Packages

`$ sudo apt update`

### Java

`$ sudo add-apt-repository -y ppa:webupd8team/java`

`$ sudo apt-get update`

`$ sudo apt-get install oracle-java8-installer`

## Combine source code

`$ sudo git clone https://github.com/tronprotocol/java-tron`

`$ cd java-tron`

`$ ./gradlew clean build -x test`

## Run a Full Node
`$  java -Xmx24g -XX:+UseConcMarkSweepGC -jar FullNode.jar -c main_net_config.conf`

## Run with Snapshot

`$ java -Xmx24g -XX:+UseConcMarkSweepGC -jar Snapshotdb.jar --witness -c main_net_config.conf`

Download Snapshotdb.jar at https://developers.tron.network/docs/main-net-database-snapshots

