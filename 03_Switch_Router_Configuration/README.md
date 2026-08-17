# Basic Switch & Router Configuration

## Objective

Configure and verify basic Cisco switch and router settings using Cisco Packet Tracer.

## Topology

PC0 ─── Switch ─── Router
## Devices

- 1 × PC
- 1 × Cisco 2960 Switch
- 1 × Cisco 1941 Router

## IP Configuration

### PC0

- IP Address: 192.168.1.10
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.1.1

### Router

Interface: GigabitEthernet0/0

- IP Address: 192.168.1.1
- Subnet Mask: 255.255.255.0

## Router Configuration

Configured the router with:

hostname R1
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
## Switch Configuration

Configured the switch hostname:

hostname SW1
## Verification

Used:

show ip interface brief
to verify the router interface status and IP address.

Used:

show running-config
to verify the current configuration.

Used:

show mac address-table
to verify MAC address learning on the switch.

## Connectivity Test

Tested connectivity from PC0 to the router:

ping 192.168.1.1
## What I Learned

- Cisco IOS command modes
- enable and privileged EXEC mode
- configure terminal and global configuration mode
- Configuring a device hostname
- Entering interface configuration mode
- Assigning an IPv4 address to a router interface
- Enabling an interface using no shutdown
- Verifying interfaces using show ip interface brief
- Viewing the running configuration
- Verifying MAC address learning on a switch
- Testing connectivity using ping

## Tools

- Cisco Packet Tracer
