--
layout: post
title:  "Develop A RESTCONF Application for Brocade Vyatta Controller (BVC) 1.1.1"
date:   2015-02-10 16:26:55
categories: jekyll update devops netdev appdev
author:  jim_burns
---

If you have followed the previous blogs you already have a BVC connected to a mininet and you are itching to get started 
writing an application that will monitor, manage and control your network.  This post will teach you how to write 
a simple application that demonstrates using the RESTCONF interface to BVC 1.1.1.

The final application can be cloned from https://github.com/jebpublic/bvcRestConfExample1 using the command:

 * git clone https://github.com/jebpublic/bvcRestConfExample1.git

There are two videos that discuss the development of this application.  The first discusses setting up the Python
development environment and Google Chrome Postman.  The second video dicusses the research and then provides a code
walkthrough as well as an example execution.


This video demonstrates how to setup a development environment:

<iframe width="560" height="315" src="https://www.youtube.com/embed/m-ZQF9obn60" frameborder="0" allowfullscreen></iframe>


This video discusses the research for the application and provides a code walkthrough and demonstration:

<iframe width="560" height="315" src="https://www.youtube.com/embed/hLLlhmuAR2Y" frameborder="0" allowfullscreen></iframe>


Download Links:

 * <a href="https://github.com/BRCDcomm/BVC/blob/master/docs/bvc-1.1.1-user-guide.pdf?raw=true" target="_blank">BVC User Guide</a>
 * <a href="https://www.getpostman.com/collections/313544e6800827de2d80" target="_blank">BVC Postman Collection</a>
 * <a href="https://wiki.opendaylight.org/view/OpenDaylight_Controller:MD-SAL:Restconf:Change_event_notification_subscription" target="_blank">Change Event Notification Subscription</a>
 * <a href="https://github.com/opendaylight/controller/tree/master/opendaylight/md-sal/model" target="_blank">OpenDaylight Controller Yang Models</a>
 * <a href="https://github.com/opendaylight/yangtools/tree/master/model/ietf" target="_blank">OpenDaylight Yangtools IETF Models</a>
 * <a href="https://wiki.opendaylight.org/view/Editing_OpenDaylight_OpenFlow_Plugin:End_to_End_Flows:Example_Flows" target="_blank">OpenDaylight Flow Examples</a>


Related Blog Posts:

 * [Install Brocade Vyatta Controller 1.1.1][InstallBVC]
 * [Install and Connect Mininet][InstallMininet]

More Info Links:

 * <a href="https://github.com/BRCDcomm/BVC/wiki" target="_blank">BVC Wiki</a> is where you can find out more information about BVC 1.1.1.
 * <a href="http://community.brocade.com/t5/DevNet/ct-p/APISupport" target="_blank">Brocade Vyatta DevNet Community</a> is where you can find discussions and docs about BVC and programming it.

[InstallBVC]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/01/19/install-brocade-vyatta-controller.html
[InstallMininet]: http://brcdcomm.github.io/BVC/jekyll/update/devops/netdev/appdev/2015/01/28/install-connect-mininet-to-bvc.html

