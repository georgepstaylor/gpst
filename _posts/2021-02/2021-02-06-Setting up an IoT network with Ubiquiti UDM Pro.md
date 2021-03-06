---
title: Setting up an IoT network with Ubiquiti UDM Pro
layout: post
headerimg: https://images.unsplash.com/photo-1520869562399-e772f042f422?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=2552&q=80
heroimg: https://images.unsplash.com/photo-1451187580459-43490279c0fa?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=2104&q=80
featured: yes
category: write
tags: ubiquiti networking
tag_colors: 
- '#0093D7'
- navy
---

# Segmentation

Within networking, the concept of segmentation involves splitting a networking into multiple sub-networks (subnets).

# Creating a new network

![Creating a new network](iotnet-1.png)

## DHCP range

Changing the DHCP range for your new network is reccomended so that the devices are on a different subnet.

## VLAN Tagging

# Using the network

## WiFi
vlan tagging ssid
## Switch ports

# Enabling the mDNS reflector 

![mDNS Setting](iotnet-2.png)

For devices such as Amazon Echo or a Chromecast, multicast DNS reflector must be enabled for so that they can discover devices on the network. The reason the reflector option exists is because the mDNS service doesn't function across multiple VLANs - the mDNS refelctor allows for multicast DNS to operate on multiple VLANs.

