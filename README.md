Reliable Data Transfer System for Online Banking
Overview
This project demonstrates a reliable data transfer system for online
banking. It focuses on detecting transmission errors and supporting
accurate communication between banking clients and a central banking
server.

The network is designed and simulated in Cisco Packet Tracer. It
includes five client PCs connected to a switch and router, a serial WAN
link between two routers, and a server-side LAN containing the banking
server.
Project Objectives
- Design a client-server network for banking communication.
- Use Cyclic Redundancy Check (CRC) to detect errors in data frames.
- Demonstrate how a receiver accepts or rejects a frame based on the
  CRC remainder.
- Explain error control, retransmission using ARQ, and flow control.
- Verify connectivity between the client network and the banking
  server.
CRC Demonstration
The report uses the following data:
- Data bits: 1101011011
- Generator polynomial: 10011
- CRC remainder: 1110
- Transmitted frame: 11010110111110
When the frame is received without error, the CRC remainder is 0000
and the frame is accepted. In the demonstrated error case, a changed bit
produces a non-zero remainder, so the corrupted frame is rejected. ARQ
may be used to request retransmission.
Network Topology
The simulated path is:

PC0 → Switch0 → Router0 → Serial WAN Link → Router1 → Switch1 → Server0

The client LAN uses the 172.16.10.0/24 network, the server LAN uses
172.16.20.0/24, and the routers communicate over the 10.10.10.0/30
WAN link. Static routes are configured on both routers.
Tools and Technologies
- Cisco Packet Tracer
- PCs, switches, routers, and a server
- CRC error detection
- Static routing
- ARQ and flow-control concepts
Expected Outcome
The Packet Tracer simulation verifies communication between a client PC
and the banking server. The CRC example demonstrates how transmission
errors can be detected and corrupted frames rejected, helping explain
reliable data transfer in an online banking network.
Future Improvements
Possible extensions include network redundancy, VLANs, advanced routing,
encryption, authentication, IDS/IPS, real-time monitoring, cloud
services, and disaster recovery.
