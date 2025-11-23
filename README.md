# Network-Design-and-Topology-Creation-Cisco-Packet-Tracer-

## Date:21-11-2025
## Name : jenil pio j
## Reg No :212223220040

## AIM:
To design a scalable multi-router network that demonstrates effective LAN and WAN integration, ensuring all devices can communicate seamlessly while exploring routing configuration and packet flow analysis in Cisco Packet Tracer.

✔ Verification of successful communication (Ping / Simulation mode)
## TOPOLOGY DIAGRAM :

<img width="1914" height="1085" alt="Screenshot 2025-11-17 173135" src="https://github.com/user-attachments/assets/58b08e94-f711-4285-b795-828dcc7f904f" />


## DESCRIPTION:

This network topology represents a small enterprise network designed using Cisco Packet Tracer.
The network consists of three routers (Router0, Router1, Router2) connected in a serial WAN topology.
Each router connects to a LAN through a switch, and every LAN contains two PCs.

This network simulates a small enterprise environment consisting of three interconnected routers, each linked to a dedicated LAN. Each LAN includes two PCs connected through a switch, representing different departments or office segments. The routers are connected using serial point-to-point links, creating a WAN backbone that enables communication between all LANs.

The network is structured to:

Assign unique IP subnets to each LAN for organized addressing.

Establish WAN links with /30 subnets to minimize IP wastage.

Configure routing (static or dynamic) to allow PCs in different LANs to communicate.

Enable monitoring and verification of data flow using ping tests and simulation mode.

This setup provides hands-on experience in network design, IP addressing, routing configuration, and troubleshooting within a multi-router enterprise topology.

Each LAN uses unique IPv4 networks:

LAN 1 (Router0):
192.168.0.0/24 and 192.168.1.0/24

LAN 2 (Router1):
192.168.1.0/24 and 10.10.1.0/24

LAN 3 (Router2):
192.168.10.0/24 and 10.10.2.0/24

Routers are interconnected using point-to-point networks:

12.12.0.0/30 between Router0 ↔ Router1

15.15.0.0/30 between Router1 ↔ Router2

The purpose of this topology is to enable end-to-end communication between all PCs through proper router configuration and routing.

## PROCEDURE :
#### Step 1: Create the Topology

Place three 2911 routers

Connect each router to a 2960 switch

Add two PCs per LAN

Connect routers with Serial DCE/DTE cables

#### Step 2: Assign IP Addresses

Configure IP addresses on PCs

Configure LAN interfaces on routers (GigabitEthernet0/0)

Configure WAN serial interfaces with /30 networks

#### Step 3: Configure Routing

Use either Static Routing or RIP/OSPF.

(Example: Static Routing)
On Router0:

ip route 192.168.1.0 255.255.255.0 12.12.0.2
ip route 192.168.10.0 255.255.255.0 12.12.0.2
ip route 10.10.1.0 255.255.255.0 12.12.0.2
ip route 10.10.2.0 255.255.255.0 12.12.0.2


(Repeat similar routes on Router1 and Router2.)

#### Step 4: Test Connectivity

Use ping, e.g., from PC0 → PC4

All devices should reply successfully

Use Simulation mode to observe packet movement

## OUTPUT :


##### PC-0 and PC-1 :
<img width="1918" height="1082" alt="image" src="https://github.com/user-attachments/assets/6f91c45c-eec3-44be-a3a9-59f73d6b9701" />

##### PC-2 and PC-3 :

<img width="1918" height="1138" alt="image" src="https://github.com/user-attachments/assets/141a5ec1-806c-4b6a-9ab0-a08b3a6a3b2d" />

##### PC-4 and PC-5 :

<img width="1918" height="1142" alt="image" src="https://github.com/user-attachments/assets/6782908b-a08e-4c57-b4a3-c08a408f1878" />
##### Router -0 :

<img width="1918" height="1140" alt="image" src="https://github.com/user-attachments/assets/5b56b318-57d3-4cae-969e-75bc930a18db" />

##### Router-1 :

<img width="1918" height="1060" alt="image" src="https://github.com/user-attachments/assets/bd9e7e72-b346-4b2f-9c60-7ec33ed040dd" />

##### Router-2 :

<img width="1915" height="1137" alt="image" src="https://github.com/user-attachments/assets/cdffc67c-bf1c-4864-bd32-ca2953339bda" />


## RESULT :

✔ The enterprise network was successfully designed and implemented in Cisco Packet Tracer.

✔ All routers communicated using properly configured WAN links.

✔ All LAN PCs could communicate with each other across different networks.

✔ Routing configuration ensured end-to-end reachability between all three network segments.

✔ The topology demonstrates the practical working of LAN/WAN design, router configuration, and routing protocols.
