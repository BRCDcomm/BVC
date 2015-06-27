---
layout: post
title:  "Develop A RESTCONF Application for NETCONF Device (vRouter 5600) via Brocade SDN Controller Using pybvc Library"
date:   2015-03-01 16:26:55
categories: jekyll update devops netdev appdev
author:  jim_burns
---

If you have followed the previous blogs you have a Brocade SDN Controller installed and have used it to program
OpenFlow flows to a Mininet virtual switch.  But, what about all this talk of NETCONF?
This post will demonstrate how to write a simple application that use the RESTCONF api of Brocade SDN
Controller to connect a Brocade vRouter 5600 to Brocade SDN Controller via NETCONF and then to add/remove a firewall.
It also introduces the pybvc Python library that wraps the RESTCONF calls and makes your applications a bit
easier to read.


<iframe width="560" height="315" src="https://www.youtube.com/embed/bekvTtMpuUo" frameborder="0" allowfullscreen></iframe>


Download Links:

 * <a href="https://github.com/brcdcomm/pybvc" target="_blank">pybvc Github repository</a>
 * <a href="https://github.com/brcdcomm/pybvcsamples" target="_blank">pybvcsamples Github repository</a>
 * <a href="https://github.com/brcdcomm/pybvccmds" target="_blank">pybvccmds Github repository</a>


Related Blog Posts:

 * [Install Brocade SDN Controller][InstallBVC]
 * [First RESTCONF Application For OpenFlow Device (Mininet)][ProgramOpenFlow]

More Info Links:

 * <a href="https://github.com/BRCDcomm/BVC/wiki" target="_blank">Brocade SDN Controller Wiki</a> is where you can find out more information about Brocade SDN Controller.
 * <a href="http://community.brocade.com/t5/DevNet/ct-p/APISupport" target="_blank">Brocade SDN Controller DevNet Community</a> is where you can find discussions and docs about Brocade SDN Controller and programming it.

[InstallBVC]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/01/19/install-brocade-vyatta-controller.html
[ProgramOpenFlow]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/02/10/restconf-app-1.html
