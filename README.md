Mininet Mobile: Rapid Prototyping for Software Defined Mobile Networks
======================================================================
**Mininet Mobile** is an extension to Mininet (<http://mininet.org>) 
aimed for emulating SDN mobile networks. It emulates large scale networks
of mobile nodes, links, and OpenFlow switches across several machines. 

## How does it work?
Mininet creates virtual networks using process-based virtualization
and network namespaces - features that are available in recent Linux
kernels. In Mininet, hosts are emulated as `bash` processes running in
a network namespace, so any code that would normally run on a Linux
server (like a web server or client program) should run just fine
within a Mininet "Host".  The Mininet "Host" will have its own private
network interface and can only see its own processes.  Switches in
Mininet are software-based switches like Open vSwitch or the OpenFlow
reference switch.  Links are virtual ethernet pairs, which live in the
Linux kernel and connect our emulated switches to emulated hosts
(processes).

## New features in this release
**Mininet Mobile** provides several new features, including:
* A new user-friendly GUI which enables visualization of large scale
networks, highlighting of flows between end hosts, remote connection to
a running instance of Mininet, dynamically change the network topology
during runtime...
* A new class of node `Mobile`, which can be moved from one switch to another
during runtime
* Enhanced cluster support
