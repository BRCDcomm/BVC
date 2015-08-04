---
layout: post
title:  "OpenStack (PackStack) with Brocade SDN Controller Part 1 - Preparation"
date:   2015-08-07 16:26:55
categories: jekyll update devops netdev appdev
author:  uwe_dahlmann
---

This video is part one (1) in a series of videos that will walk you through setting up OpenStack with the Brocade SDN Controller.  This video walk you through setting up the virtual machines and network connections between them as preparation for later videos.

<iframe width="560" height="315" src="https://www.youtube.com/embed/RgspYJaUkBw" frameborder="0" allowfullscreen></iframe>

Related Commands:

```
ip addr show
systemctl stop NetworkManager
```

```
Systemctl disable NetworkManager
sudo yum remove NetworkManager
chkconfig network
dhclient
ifup eth0
ifup eth1
sudo yum install net-tools
 
cd /etc/sysconfig/network-scripts
vi ifcfg-eth0
	change onboot to yes
	change Peerdns to no
	Vi: I for insert, type whatever, esc to end typing, :x to save:: :q! to exit without saving
	same for ifcfg-eth1
 
vi /etc/resolv.conf
nameserver 8.8.8.8
nameserver 8.8.4.4
 
shutdown -r now
```

Related Videos:

* <a href="https://www.youtube.com/watch?v=blfWoIiMqb0" target="_blank">Install Brocade SDN Controller</a>

Download Links:

* <a href="http://store.brocade.com" target="_blank">Download Brocade SDN Controller</a>


More Info Links:

 * <a href="https://github.com/BRCDcomm/BVC/wiki/RESTCONF-Developer-Resources" target="_blank">Brocade SDN Controller RESTCONF Developer Resources</a> is where you can find tools, info and samples for programming Brocade SDN Controller via the RESTCONF API
 * <a href="https://github.com/BRCDcomm/BVC/wiki" target="_blank">Brocade SDN Controller Wiki</a> is where you can find out more information about Brocade SDN Controller.
 * <a href="https://brcdcomm.github.io/BVC/" target="_blank">Brocade SDN Controller Blog</a> is where you can find articles and videos about Brocade SDN Controller.
 * <a href="http://community.brocade.com/t5/DevNet/ct-p/APISupport" target="_blank">Brocade SDN Controller DevNet Community</a> is where you can find discussions and docs about Brocade SDN Controller and programming it.

[InstallBVC]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/01/19/install-brocade-vyatta-controller.html
[ProgramOpenFlow]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/02/10/restconf-app-1.html
