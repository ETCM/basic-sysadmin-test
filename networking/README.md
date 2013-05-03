Networking Architecture, Design and Maintainence
================================================

Please answer the following questions.

Q1) What are the OSI layers and how do they relate day-to-day operations?
-------------------------------------------------------------------------
The OSI layers are part of the OSI model. This model is used to create a conceptual view of network communications. It provides a representation of the relation between the adjacent layers.
* Application    - Layer 7
* Presentation   - Layer 6
* Session        - Layer 5
* Transport      - Layer 4
* Network        - Layer 3
* Data Link      - Layer 2
* Physical       - Layer 1

The OSI layers can be used in everyday network troubleshooting to narrow down the search area for certain issues such as application or hardware connectivity problems. It can also be used to make design issues within a network.

Q2) Cisco/Juniper/Equivalent: Pick one and explain how to configure a VLAN.
---------------------------------------------------------------------------

Q3) What is the difference between an application switch and a layer-2/3 switch?
--------------------------------------------------------------------------------
A layer 2/3 switch is typically only used for functions such as switching, routing and network address translation. Application switches (layer 7) are more complex and can be used for full packet inspection, application filtering, load balancing, etc. 

Q4) How does virtualization interact with network design?
---------------------------------------------------------


Q5) TCP Handshake. What is it?
------------------------------
The TCP handshake is the process used by TCP packets during transmission. It is a protocol that must be followed for establishment of a connection between a client and server. 

The originator sends a SYN packet to the destination
The desitnation subject responds by sending a SYN-ACK packet back to the originator
The originator sends an ACK to the destination for acknowledgement

Failure of this protocol can cause retransmission of packets.

Q6) What is the difference between a MAC address and an IP address?
-------------------------------------------------------------------
A MAC address is a hardware identifier that is primarily used for layer-2 network addressing. An IP address is a logical layer-3 address that is used for routing traffic both within and outside of the originating network. Since MAC addressing is a layer 2 protocol it can not be used to route traffic to the internet or other networks. IP addressing has this ability and is not tied to the hardware in the same way as a MAC address.

Q7) ARP Storm vs ARP Poisoning. Compare and Contrast.
-----------------------------------------------------
Both the ARP storm and ARP poisoning attempt to leverage the vulnerabilities of the address resolution protocol in order to compromise a device on the network. The attacks both allow the attacker to mount a DoS attack.

ARP poisoning occurs when the attacker spoofs a valid IP address on the network so that it can be associated with the attacker's MAC address. This allows network traffic meant for the spoofed address to be routed to the attacker. 

ARP storm is created when an attacker sends out broadcast packets to internal IP addresses.


Q8) Scenario Response:
----------------------
Your organization's network administrator contacts you, noting that a host using IP 192.168.100.106 is flooding the network.  You decide to take that host offline in the short term to prevent additional flooding.  Your network uses Cisco switches.  How would you identify which port to shut down?

You can use the MAC address table on the switch to find out which port is associated with the host. You will first need to obtain the MAC address of the host which is causing the issues.


