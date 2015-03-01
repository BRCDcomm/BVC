---
layout: post
title:  "Develop A RESTCONF Application for NETCONF Device (vRouter 5600) via Brocade Vyatta Controller (BVC) Using pybvc Library"
date:   2015-02-10 16:26:55
categories: jekyll update devops netdev appdev
author:  jim_burns
---

If you have followed the previous blogs have a Brocade Vyatta Controller installed and have used it to program
OpenFlow flows to a Mininet virtual switch.  But, what about all this talk of NETCONF?
This post will demonstrate how to write a simple application that use the RESTCONF api of Brocade Vyatta
Controller to connect a Brocade Vyatta vRouter 5600 to BVC via NETCONF and then to add/remove a firewall.
It also introduces the pybvc Python library that wraps the RESTCONF calls and makes your applications a bit
easier to read.



The final application can be cloned from https://github.com/jebpublic/bvcRestConfExample1 using the command:

 * git clone https://github.com/jebpublic/bvcRestConfExample1.git

<iframe width="560" height="315" src="https://www.youtube.com/embed/bekvTtMpuUo" frameborder="0" allowfullscreen></iframe>


Download Links:

 * <a href="https://github.com/jebpublic/pybvc" target="_blank">pybvc Github repository</a>
 * <a href="https://github.com/jebpublic/pybvcsamples" target="_blank">pybvcsamples Github repository</a>
 * <a href="https://github.com/jebpublic/pybvccmds" target="_blank">pybvccmds Github repository</a>


Related Blog Posts:

 * [Install Brocade Vyatta Controller 1.1.1][InstallBVC]
 * [First RESTCONF Application For OpenFlow Device (Mininet)][ProgramOpenFlow]

More Info Links:

 * <a href="https://github.com/BRCDcomm/BVC/wiki" target="_blank">BVC Wiki</a> is where you can find out more information about BVC 1.1.1.
 * <a href="http://community.brocade.com/t5/DevNet/ct-p/APISupport" target="_blank">Brocade Vyatta DevNet Community</a> is where you can find discussions and docs about BVC and programming it.

[InstallBVC]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/01/19/install-brocade-vyatta-controller.html
[ProgramOpenFlow]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/02/10/restconf-app-1.html
