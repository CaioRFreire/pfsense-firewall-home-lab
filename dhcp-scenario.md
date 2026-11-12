# 1. DHCP Server Configuration

## Objective

In this scenario, I have configured the pfSense DHCP server to automatically assign IP addresses to devices connected to the internal `labnet` network. Since we just have the Ubuntu machine on the `labnet` network, the IP address will be assigned to it.

## Configuration

The DHCP server was enabled and configured through the pfSense web interface under **Services / DHCP Server / LAN**.

<p align="left">
  <img src="dhcp-server-images/dhcp server pfsense conf.png" width="70%">
</p>

## Validation

The Ubuntu Machine was configured to obtain its IP address automatically. The `ifconfig` command was used to verify the assigned address.


<p align="left">
  <img src="dhcp-server-images/dhcp ubuntu ip assigned.png" width="70%">
</p>

The Ubuntu Machine successfully received the IP address `192.168.1.100` from the pfSense DHCP server.

## Result

Automatic IP address assignment was successfully validated on the Ubuntu machine. 

DHCP simplifies network administration by eliminating the need for manual IP configuration and reducing the risk of address conflicts.

