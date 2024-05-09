# Cisco Packet Tracer Project - SOHO Network Design
Subnetting for a Small SOHO Network

As an exercise, I decided to build a small office network with two departments – one for accounting and one for sales. This would be disturbingly small representation of a company so we will pretend it’s merely one arm of a network inside a larger building. For my topology, each subnetwork had the following:
2 PCs
1 printer
1 switch
1 router

To see the subnetting calculations in depth, please see my documentation in the files or read my [blog post](https://pattychungcouk.wordpress.com/2023/10/29/subnetting-a-small-office-network-in-cisco-packet-tracer/).

## Network topology
![small-network-all-ips-configed](https://github.com/pattytechuk/CPT-Small-SOHO-Network/assets/167561785/51734a46-9b7a-4a2d-bde4-fb6976866b9c)

## Network device configuration

Enabled both interfaces for the router and assigning IP to Gig 0/0 and Gig0/1:
![image](https://github.com/pattytechuk/CPT-Small-SOHO-Network/assets/167561785/4a5acd7a-17eb-4dc6-b824-91023ed32944)
![image](https://github.com/pattytechuk/CPT-Small-SOHO-Network/assets/167561785/4ca3388d-58e4-4325-b58b-ed7c24158c69)

## Testing communication between subnets
Going into Command Line on PC0 (on subnet 1), I pinged PC2 on subnet 2:
![ping-from-pc0-to-pc2](https://github.com/pattytechuk/CPT-Small-SOHO-Network/assets/167561785/a2a226fc-a1db-4e19-94b2-6fccfdc5ff92)

All packets returned, signaling successful communication and connection between devices.

I also pinged from PC1 (on subnet 1) to printer 1 on subnet 2:
![ping-from-pc1-to-printer1](https://github.com/pattytechuk/CPT-Small-SOHO-Network/assets/167561785/3bc01ec8-4f8b-48c6-8775-517058b252e4)

Communication between subnets was successful.
