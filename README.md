# IoT-Traffic-Generator
The udp-client.c and udp-server.c files form an embedded software application written for Contiki operating system. The goal of this application is to generate UDP traffic in an Internet of Things (IoT) testbed. The server program should be deployed on one of the IoT nodes (referred to as gateway) and the client program should be deployed on a number of other IoT nodes. Then, by running these programs, each client device will periodically (every 60 seconds) read the value of atmospheric pressure from node's sensor and will send it to the gateway over a UDP connection. In order to prevent synchronization between clients, each client node waits for a random delay before starting to generate traffic.

This application is tested with IoT devices deployed in FIT IoT-LAB testbed (https://www.iot-lab.info/). Indeed, the udp-client.c program is a modification of one of the example programs provided in that platform. The udp-server.c is the exact example provided in the platform and is included here for the completeness of the project.

The unmodified example files can  be found in the following path on FIT IoT-LAB devices:

~/iot-lab/parts/contiki.examples/ipv6/rpl-udp
