
# Client-Server Network Setup Tutorial Using Cisco Packet Tracer

## Objectives

1. Understand the basics of a client-server network.
2. Learn how to use Cisco Packet Tracer to set up a client-server network.

## Tools Required

- Cisco Packet Tracer

## Steps

### Step 1: Launch Cisco Packet Tracer

1. Open Cisco Packet Tracer on your computer.
2. Start a new project.

### Step 2: Add Network Devices and PCs

1. From the bottom-left panel, select the "End Devices" option.
2. Drag and drop two generic PCs onto the workspace for the clients.
3. Add a Server onto the workspace.

### Step 3: Add Connections

1. Click on the "Connections" icon (it looks like a lightning bolt).
2. Select the "Copper Straight-Through" cable.
3. Connect each PC to the server's FastEthernet ports.

### Step 4: Configure Server

1. Click on the server, then go to the "Services" tab.
2. Enable HTTP, FTP, or any other service you want to demonstrate.
3. Go to the "Config" tab to set up an IP address for the server, e.g., `192.168.1.10` and Subnet Mask `255.255.255.0`.

### Step 5: Configure Clients

1. Click on the first PC, then go to the "Desktop" tab.
2. Open "IP Configuration" and set an IP address (e.g., `192.168.1.1`) and Subnet Mask (`255.255.255.0`).
3. Repeat the above steps for the second client, but use a different IP address, e.g., `192.168.1.2`.

### Step 6: Test the Connection

1. Go to one of the client PCs.
2. Open a browser and enter the IP address of the server.
3. If configured correctly, you should be able to access the server's services.

### Step 7: Verify the Network

1. Use the "Add Simple PDU" or "Add Complex PDU" tool to send packets from the clients to the server and observe the behavior.

## Troubleshooting

- If you cannot connect, double-check the IP configurations and cabling.
- Use the "Simulation" mode to identify where the issue may lie.

