
# Local Area Network (LAN) Setup Tutorial Using Cisco Packet Tracer

## Objectives

1. Understand the basics of a Local Area Network (LAN).
2. Learn how to set up a simple LAN using a router and a switch in Cisco Packet Tracer.

## Tools Required

- Cisco Packet Tracer

## Steps

### Step 1: Launch Cisco Packet Tracer

1. Open Cisco Packet Tracer on your computer.
2. Start a new project.

### Step 2: Add Network Devices

1. From the bottom-left panel, select "Routers" and drag a generic router onto the workspace.
2. Select "Switches" and drag a generic switch next to the router.

### Step 3: Add End Devices

1. Go to "End Devices" and drag three generic PCs onto the workspace.

### Step 4: Add Connections

1. Use the "Connections" icon (lightning bolt) to select "Copper Straight-Through" cables.
2. Connect the router's FastEthernet0/0 port to any port on the switch.
3. Connect each PC to different ports on the switch.

### Step 5: Configure Router

1. Click on the router, go to the "Config" tab.
2. Set the IP address for FastEthernet0/0 to `192.168.1.1` and Subnet Mask to `255.255.255.0`.

### Step 6: Configure PCs

1. Click on the first PC, go to the "Desktop" tab.
2. Open "IP Configuration" and set:
    - IP Address: `192.168.1.2`
    - Subnet Mask: `255.255.255.0`
    - Default Gateway: `192.168.1.1`
3. Repeat for the remaining PCs with different IP addresses (e.g., `192.168.1.3` and `192.168.1.4`).

### Step 7: Test the Network

1. Use the "Add Simple PDU" tool to send packets between PCs.
2. If the packets reach successfully, your LAN setup is complete.

## Troubleshooting

- If the network is not functioning as expected, double-check the IP configurations and connections.
- Use the "Simulation" mode to debug any issues.

