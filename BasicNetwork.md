# Cisco Packet Tracer: Basic Networking Tutorial

## Objectives
- Understand basic networking components
- Create a Local Area Network (LAN)
- Configure routers and switches
- Connect end devices and verify connectivity using ping

## Requirements
- Cisco Packet Tracer installed
- Basic understanding of networking concepts

## Steps

### Step 1: Open Cisco Packet Tracer
Launch the program and click on `New` to create a new workspace.

### Step 2: Add Networking Devices
Drag and drop the necessary networking devices into the workspace. For this tutorial, you will need:
- 1 Router (e.g., 2911)
- 1 Switch (e.g., 2960)
- 2 PCs

### Step 3: Interconnect Devices
Use the `Connections` tool (represented by a lightning bolt icon) to connect the devices.

- **Router's Gig0/0 to Switch's Fa0/1**: Connecting the router's Gigabit port (Gig0/0) to the switch's FastEthernet port (Fa0/1) ensures that the router can communicate with the devices connected to the switch. Gig0/0 is usually the first interface on the router, and Fa0/1 is a commonly used first port on the switch.

- **PCs to Switch (Fa0/2 and Fa0/3)**: Connect each PC to a different port on the switch using straight-through cables. This establishes the local network for the PCs.

### Step 4: Configure the Router
Click on the router, go to the `CLI` tab, and enter the following commands to configure its interface:

```bash
enable
configure terminal
interface Gig0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
```
**Justification**: We configure the router's Gig0/0 interface with an IP address and bring it up (no shutdown). This acts as the gateway for the local network, allowing the PCs to communicate beyond the local network.

### Step 5: Configure the PCs
Click on each PC, navigate to the Desktop tab, and then to IP Configuration. Configure the IP settings as follows:

- PC1: IP address `192.168.1.2`, Subnet Mask `255.255.255.0`, Default Gateway `192.168.1.1`
- PC2: IP address `192.168.1.3`, Subnet Mask `255.255.255.0`, Default Gateway `192.168.1.1`
Justification: Configuring the PCs with IP addresses in the same subnet as the router allows them to communicate with each other and the router.

### Step 6 : Test Connectivity Using Ping
1. Click on the PC Device you want to ping
2. Open the Command Prompt by navigating to the `Desktop` tab and click on `Command Prompt`.
3. Execute Ping Command : Type `ping` followed by the IP address of the device you wish to ping. e.g `ping 192.168.1.3`.
4. Analyze Results: If you see replies, the device is reachable. Otherwise, you will need to troubleshoot the network.

**Justification**: Using the `ping` command verifies that the devices are properly configured and can communicate within the network. It is a simple yet effective tool for troubleshooting netweork issues. 

