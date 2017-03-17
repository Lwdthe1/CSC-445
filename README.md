# CSC-445
Doug Lea's Computer Networking Course (CSC 445)
http://gee.cs.oswego.edu/dl/csc445/

Scroll down for descriptions of my completed assignments.

## Topics Covered

* Network Structure and Implementation
* Layered Systems
* Point-to-Point and shared media
* Switching
* Internetworking
* IP and Routing
* TCP and UDP
* Socket programming
* Congestion control and Quality of Service
* Application protocols: HTTP, FTP, etc
* Distributed Systems
* RPC and remote invocation
* Naming, Security, Caching
* Group communication
* Frameworks: CORBA, Jini, etc

## Assignment 3: Distributed Systems

## Assignment 2
"Write a file upload program. To demonstrate, you'll need a client and a server program, doing the obvious.
The server awaits connections.
A client connects, sends the name of a file it wants to upload.
The client sends the file and the server stores it.
Wherever applicable, use the commands and protocol for TFTP (IETF RFC 1350), with the following modifications:

A client only sends files, never receives.
Support only binary (octet) transmission.
Support a command line argument specifiying whether packets are IPv4 vs IPv6 UDP datagrams
Support a command line argument specifying to use TCP-style sliding windows rather than the sequential acks used in TFTP. To implement this, you may need to design and use additional packet header information than that in TFTP.
Support a command line argument controlling whether to pretend to drop 1 percent of the packets;
Create a web page showing throughput across varying conditions (V4 vs V6; sequential vs windowed acks; drops vs no drops)"
http://gee.cs.oswego.edu/dl/csc445/a2.html

## Asignment 1
"Measure the latency and throughput of TCP and UDP across at least three pairs of machines using at least two different networks. For example, two CS servers (like wolf and pi), or a CS server to a laptop, wired or wireless, or off-campus. Create a web page with graphs summarizing your results. Include the following measurements:
Measure round-trip latency as a function of message size, by sending and receiving (echoing) messages of size 1, 32, and 1024 bytes. Measure RTTs.
Measure throughput by sending messages of size 1K, 16K, 64K, 256K, and 1M bytes in each direction. Measure transfer rates.
Measure the interaction between message size and number of messages (using TCP only) by sending 1MByte of data (with a 1-byte acknowledgment in the reverse direction) using different numbers of messages: 256 x 4KByte messages, 512 x 2KByte messages, 1024 x 1KByte messages, and so on.
For timing, use System.nanoTime. Read through the Java networking tutorial. Also see SimpleService.java and EchoClient.java for some stripped-down examples of using server and client sockets. When using non-CS machines and networks, minimize unnecessary traffic while developing your programs. Beware of firewalls."
http://gee.cs.oswego.edu/dl/csc445/a1.html
