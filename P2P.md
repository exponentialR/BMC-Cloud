
# Peer-to-Peer Network Setup Tutorial Using Cisco Packet Tracer

## Objectives

1. Understand the basics of a peer-to-peer network.
2. Learn how to use Cisco Packet Tracer to set up a P2P network.

## Tools Required

- Cisco Packet Tracer

## Steps

### Step 1: Launch Cisco Packet Tracer

1. Open Cisco Packet Tracer on your computer.
2. Start a new project.

### Step 2: Add Network Devices and PCs

1. From the bottom-left panel, select the "End Devices" option.
2. Drag and drop two generic PCs onto the workspace.

### Step 3: Add Connections

1. Click on the "Connections" icon (it looks like a lightning bolt).
2. Select the "Copper Straight-Through" cable.
3. Click on the first PC and connect it to the FastEthernet0 port.
4. Click on the second PC and connect it to its FastEthernet0 port.

### Step 4: Configure PCs

1. Click on the first PC, then go to the "Desktop" tab.
2. Open "IP Configuration" and set the following:
    - IP Address: `192.168.1.1`
    - Subnet Mask: `255.255.255.0`
3. Click "Save" or "Close" to exit.
4. Repeat the above steps for the second PC, but use the IP address `192.168.1.2`.

### Step 5: Test the Connection

1. Go back to the workspace.
2. Click on the "Add Simple PDU" icon (it looks like a packet envelope).
3. Click on the first PC, then on the second PC, to send a packet.

### Step 6: Verify the Network

1. If the packet successfully reaches the second PC, you'll see a checkmark, confirming that the P2P network is functional.

## Troubleshooting

- If the packet doesn't reach its destination, double-check the IP configuration and cabling.
- Use the "Simulation" mode to observe packet transfer in detail and identify any issues.

