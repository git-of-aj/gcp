# VPC
## Basics
- A Virtual Private Cloud (VPC) network is a virtual version of a physical network
- A VPC network does the following:

1. Provides connectivity for your Compute Engine virtual machine (VM) instances.
2. Offers native internal passthrough Network Load Balancers and proxy systems for internal Application Load Balancers.
3. Connects to on-premises networks by using Cloud VPN tunnels and VLAN attachments for Cloud Interconnect.
4. Distributes traffic from Google Cloud external load balancers to backends.

- Projects can contain multiple VPC networks.
- Unless you create an organizational policy that prohibits it,new projects start with a **default network (an auto mode VPC network) that has one subnetwork (subnet) in each region.**
![](https://cloud.google.com/static/vpc/images/vpc-overview-example.svg)
## VPC
- VPC networks, including their associated routes and firewall rules, are global resources. They are not associated with any particular region or zone.
- Subnets are regional resources (each subnet can have different IPv4)
- An organization can use Shared VPC to keep a VPC network in a common host project. Authorized IAM principals from other projects in the same organization can create resources that use subnets of the Shared VPC network
-
## Subnet
- When an auto mode VPC network is created, one subnet from each region is automatically created within it. New Region ==> Subnet Auto added
- When a custom mode VPC network is created, no subnets are automatically created
- switch a VPC network from auto mode to custom mode. This is a one-way conversion; custom mode VPC networks cannot be changed to auto mode VPC networks.

[GCP Auto MOde Vs Custom - Whats Good for Prod](https://cloud.google.com/vpc/docs/vpc#auto-mode-considerations)

**[VPC Communication within VPC and internet](https://cloud.google.com/vpc/docs/vpc#intra_vpc_reqs)**

## Routes
Routes define paths for packets leaving instances (egress traffic) i.e going out of network
- Dynamic routing mode: Cloud Router is a fully distributed and managed Google Cloud service that uses the Border Gateway Protocol (BGP) to advertise IP prefixe

## Firewall 
- Hierarchical firewall policies are created at the organization and folder level. Creating a policy does not automatically apply the rules to the organization or folder.
- Regional network firewall policies: Attched to VPC : can explicitly deny or allow connections, or go to the next level of the hierarchy.
- These policies contain rules that can explicitly deny or allow connections, or go to the next level of the hierarchy.
![](https://cloud.google.com/static/firewall/images/firewall-policies/hfw3-2.svg)
