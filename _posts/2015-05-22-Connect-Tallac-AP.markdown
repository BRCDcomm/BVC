---
layout: post
title:  "Connect Tallac AP to Brocade SDN Controller"
date:   2015-05-21 16:26:55
categories: jekyll update devops netdev appdev
author:  uwe_dahlmann
---

Connecting Tallac Acces Points to the Brocade Vyatta Controller:

The Tallac Access Points are a good choice for getting first experiences with wireless SDN solutions. These Access Points are cloud managed, and additionally support the OpenFlow 1.3 standard. This allows the Brocade Vyatta controller to manage dataplane forwarding on these devices, and gives the users access to the network applications written on the BVC controller.

Many controllers have problems working with devices that only have one Ethernet port, as access points often have. In this case, the controllers need to support inband control planes for these devices, which often creates problems.
Luckily, Tallac Access Points provide two Ethernet ports, and by that allow an easy way around this problem using their so called “Gateway mode”. In this mode, the Access Point uses its eth1 interface to connect the control and management plane, whereas the radios and the ethernet0 port get natted to the address received on eth1. This works exactly as the out of band connections often used for wired openflow switches.

We will now walk through all the steps necessary to connect a Tallac AP to the BVC Controller. In this example, the BVC controller is already installed and running at the IP Address 192.168.201.4. The access point is in default mode, with eth0 connected into this network. The network itself is natted to the outside world be a router. We can see our AP in the standard cloud management console www.tallac.com. As you can see the Access point is connected to the cloud management, and has the IP 192.168.88.144. 

![My helpful screenshot](http://brcdcomm.github.io/BVC/assets/TallacMgmtGUI1.png)
