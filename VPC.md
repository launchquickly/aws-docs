# VPC

Virtual Private Cloud  

It is a logical data center, effectively a virtual network. Selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can leverage multiple layers of security, including security groups and network access control lists to help control access to Amazon EC2 instances in each subnet. You can also create Hardware VPN connection between your corporate datacenter and your VPC to use AWS to extend your corporate datacenter.

- VPCs do not span Regions but can span Availability Zones
- Maximum addressable IP range is /16

## Default VPC

- Provided for each region for each account
- All Subnets have route to internet 
- if you delete VPC only way to restore is to contact AWS for support

## VPC Peering

Connect one VPC with another via a direct network route using private IP addresses

- instance behave as if they are on the same private network
- can peer VPC's with other AWS accounts as well as with VPC's in the same account
- always Star configuration - no Transitive peering

## Internet Gateway

- Attached to VPC
- Only one per VPC
- traffice to/from Internet

## Virtual Private Gateway 

- traffic to/from VPN

## Route Tables

- Configured between subnets

## Network Access Control Lists

- Stateless - inbound rules not mirrored by outbound

## Security Group

- Stateful - inbound rules mirrored by outbound

## Subnets

- Assign IP address ranges to
- 1 Subnet = 1 Availability Zone




