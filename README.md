## TCP-UDP-Viewer
TCP/UDP sockets real-time monitor (SNMP) written in Java as a school assignment

## Requirements
- [Java SE Development Kit 8 or higher](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html)
- [GNS3](https://www.gns3.com/)
- [SNMP4J SNMP Java API](https://www.snmp4j.org/)

## Network configuration

Topology of a network simulated in GNS3 is given in the following screenshot:

<p  align="center">
<img src="" 
 width="80%">
</p>

Every router in the network has SNMP and BGP configured. SNMP versions 1 and 2c are supported. Loopback addresses of the routers (where SNMP is configured) are

- 192.168.10.1 for R1;
- 192.168.20.1 for R2;
- 192.168.30.1 for R3;

but the application communicates with R1 only, which has http server configured for testing purposes.

Before using the application, the ip route table of the host machine (from the picture) must be modified so it contains neccessary routes from the network. That can be done manually, or by executing <b>setup.sh</b> script.

## Example of running application

<p  align="center">
<img src="" 
 width="80%">
</p>
