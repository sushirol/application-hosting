---
published: true
date: '2016-06-06 00:13 -0700'
title: 'XR Toolbox: Bring your own Container App'
author: Akshat Sharma
excerpt: Bring up your own Container (LXC) + Application on IOS-XR
tags:
  - vagrant
  - iosxr
  - cisco
  - linux
  - containers
  - LXC
  - iperf
---

{% include base_path %}
{% include toc icon="table" title="Bring your own Container" %}


## Introduction

The Techdoc: [Application Hosting on IOS-XR]({{ base_path}}/techdocs/app_hosting_on_iosxr/introduction) dives deep into the IOS-XR architecture, to help explain how a user can deploy an application:  

*  natively (inside the XR process space) OR
*  as a container (LXC)


In this quick start guide we use the IOS-XR vagrant box to bring up an Ubuntu container on IOS-XR and host an application within it.

So, let's get started!


## Pre-requisites

Meet the pre-requisites specified in the [IOS-XR Vagrant Quick Start guide: Pre-requisites]({{ base_path }}/tutorials/iosxr-vagrant-quickstart#pre-requisites) 
 


## Bring up the XR Vagrant instance  


We'll just need a single XR instance for this guide, so follow the  [Single Node Bringup ]({{ base_path }}/tutorials/iosxr-vagrant-quickstart#single-node-bringup) section to bring up a single XR node.




