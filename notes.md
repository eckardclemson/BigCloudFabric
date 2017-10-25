Big Cloud Fabric (BCF)
---

Big Switch Network
Gurinder.Sandhu@bigswitch.com

users:
user26@bigswitch.com/csc123
admin/bsn123

Big Monitoring Fabric

BCF integrates w/ vSphere/OpenStack/Kubernetes

Hyperscale-Inspired

Networking companies didn't come up with Hyperscale.

- centeralized control
- merchant silicon (w/ proprietary ASICs)
- fabric-based

LLDP protocal in the fabric - otherwise no protocols

Up to 128 leaf switches, 6 spine switches : from 2 redundant controllers

2 leaf switches in each rack
= 64 racks

tenant centric

vSwitch:  OpenV switches used in P+V Fabric Edition
- OpenStack
- Container (Kubernetes)

P+V is licensed by switch/vswitch

everything developed "REST first", CLI/GUI connect to REST

debug mode show REST calls

- spines are not connected to other spines
- leafs within a rack are connected to each other

VRF - Virtual Routing and Forwarding

IPAM - IP Address Management - used for containers

If both controllers go down, switches go into "headless mode"

Chaos Monkey - network tester by netflix

System switch is on spine switches

Broadcom processors

ethernet fabric ECMP-like

Ubuntu underneath CLI

There is only running configuration, no startup config.  Takes effect
immediately.

Leafs switches connect to all spines

LAG:  link aggregate group

factory: ONIE Open Network Installed Network  (like BIOS for network)

leaf group can only have 2 members

if leaf switch not explicitly given leaf group, default leaf group
name is MAC

controller to switches:  IPv6 w/ link-local address

IPAM - IP address manager

LACP fallback only for PXE boot

wildcard rules:  most specific preferred, then litttle preferred

labs.bigswitch.com - Labs anytime once you register

LLDP is the communication protocol that controllers use to determine
topology

also look into LACP

Ubuntu 16.04 is underlying

interface group == bonded networks

port groups (vCenter) =? VLAN? == BigSwitch segment

vCenter integration:  polled 1/hr and events on VCenter side sent to
BSN

LLDP preferred over CDP to communicte w/ vSphere

mininet is software for SDN - virtual switches, routers, etc

analyitics is ElasticSearch

what is Lucene query syntax?


