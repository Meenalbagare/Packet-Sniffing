# Packet-Sniffing

# ABSTRACT
Packet sniffing is a technique whereby packet data flowing across the network is 
detected and observed. It is the practice of gathering, collecting, and logging some 
or all packets that pass through a computer network, regardless of how the packet is 
addressed.
In networking, the data is transferred in the form of packets, or small chunks of 
data. These packets vary in their format, depending on the network protocol 
(TCP/IP, UDP, etc.). In addition to the actual information or data, all packets 
contain control information designed to help in the delivery of packets from source 
to destination.

# SCOPE OF THE PROJECT
Packet sniffing is used to monitor traffic running through a network. It can be used 
to understand the source host, destination host and type of protocol used.
Traffic can be analysed and the responses received for requests.
Packet sniffing is typically used for network troubleshooting. Packets detected on a 
network they are not supposed to be in might suggest improper routing or 
switching. Packets marked for ports that do not match their protocol might also 
suggest a misconfiguration of one or more nodes.
Packets can also be analysed to see if a specific application is using too much 
bandwidth or if authentication is requiring numerous back-and-forth calls.
Network administrators can monitor their network traffic and gain valuable insights 
about their infrastructure and its performance. It allows them to measure the traffic 
flow in a network and also identify which applications are using the maximum 
bandwidth.
Packet sniffing may be useful in increasing network security. When monitoring 
traffic for clear-text usernames and passwords, for example, you could notice 
possible security issues before any hacker. In addition, monitoring remote traffic 
can help ensure that all traffic is properly encrypted and not being sent out onto the 
open internet without encryption.

# PROJECT DESCRIPTION
A simple packet sniffer is implemented using the socket module using Python. The 
project can be used to monitor traffic running through a network. It can be used to 
understand the source host, destination host and type of protocol used.
The project filters TCP/IP, UDP and ICMP packets. The following features are displayed
for each protocol:
# TCP
1. Version: To differentiate between IPv4 and IPv6.
2. Header Length: TCP wraps each data packet with a header containing 10 
mandatory fields totalling 20 bytes.
3. TTL (Time to live): The value for the period of time that a packet, or data, should 
exist on a computer or network before being discarded.
4. Protocol Number: There are a number of predefined protocol numbers that are 
registered with the Internet Assigned Numbers Authority (IANA). For a 
comprehensive list of all the upper-layer Protocol Identifier numbers.
The protocol number for TCP is 6.
5. Source IP Address: The IP packet field containing the IP address of the 
workstation from which it came. The address is 32 bits long indicating it is a IPv4 
address.
6. Destination IP address - the IP packet field containing the IP address of the 
workstation to which it is addressed. The address is 32 bits long indicating it is a 
IPv4 address.
7. Source Port Number: It is used to identify the process that sent the data. The
source port number is 2 bytes long.
8. Destination Port Number: It is used to identify the process that is to receive the 
data. The destination port number is 2 bytes long.
9. Sequence Number: The sequence number is a counter used to keep track of every 
byte sent outward by a host. It is present at offset 32 into the TCP header is the 
sequence number.
10.Acknowledgement Number: The acknowledgment number field holds the 
sequence number of the next byte the receiver is expecting on this connection.
11.TCP flags: The flags indicate a particular connection state, provide some 
additional helpful information for troubleshooting purposes, or handle control of a 
specific connection.
The following flag numbers are displayed:
• URG - The urgent flag is used to notify the receiver to process the urgent 
packets before processing all other packets.
• ACK - The acknowledgment flag is used to acknowledge the successful 
receipt of a packet

PSH - The PSH flags instruct the operating system to send (for the sending 
side) and receive (for the receiving side) the data immediately.
• RST - RST flag indicates that connection should be immediately 
terminated.
• SYN-The SYN flag synchronizes sequence numbers to initiate a TCP 
connection.
• FIN - The finished flag means there is no more data from the sender.
12.Checksum - Checksum is a simple error detection mechanism to determine the 
integrity of the data transmitted over a network. Communication protocols like 
TCP|IP implement this scheme in order to determine whether the received data is 
corrupted along the network.

# UDP
1. Version: To differentiate between IPv4 and IPv6.
2. Header Length: UDP wraps each data packet with a header 8 bytes
3. TTL (Time to live): The value for the period of time that a packet, or data, should exist 
on a computer or network before being discarded.
4. Protocol Number: There are a number of predefined protocol numbers that are 
registered with the Internet Assigned Numbers Authority (IANA). For a comprehensive 
list of all the upper-layer Protocol Identifier numbers.
The protocol number for UDP is 17.
5. Source IP Address: The IP packet field containing the IP address of the workstation 
from which it came. The address is 32 bits long indicating it is a IPv4 address.
6. Destination IP address - the IP packet field containing the IP address of the 
workstation to which it is addressed. The address is 32 bits long indicating it is a IPv4 
address.
7. Source Port Number: It is used to identify the process that sent the data. The source
port number is 2 bytes long.
8. Destination Port Number: It is used to identify the process that is to receive the data.
The destination port number is 2 bytes long.
9. Length-Length of the UDP packet.
10. Checksum- Checksum is a simple error detection mechanism to determine the 
integrity of the data transmitted over a network. Communication protocols like UDP
implement this scheme in order to determine whether the received data is corrupted along 
the network.


![image](https://github.com/Meenalbagare/Packet-Sniffing/assets/99323366/d3d15214-e03b-4655-87b4-d7c1aa8ca041)

# FILTERING OUT UDP PACKETS

![image](https://github.com/Meenalbagare/Packet-Sniffing/assets/99323366/2a463dbb-5689-4ba4-9383-f172fd09f8c3)


# CONCLUSION
The implementation of a simple packet sniffer using Python can be a useful tool 
for gaining insight into network traffic. The project can be used for the real-time 
capture and analysis of network traffic, providing valuable information about the 
types of traffic flowing through a network. 
With the ability to troubleshoot network issues, analyse network protocols, 
identify security threats, measure network performance, and optimize network 
resources, packet sniffers play a crucial role in ensuring the smooth and efficient 
operation of computer networks.
While there are some risks associated with the use of packet sniffers, when used 
responsibly and ethically, they serve as a valuable tool for understanding and 
improving network performance and security


