# EC2

Elastic Compute Cloud

- Provides resizable compute capacity  
- Provides scalable infrastructure  


On Demand - allow you to pay fixed rate by the hour with no commitement  
Reserved - provide with a capacity reservation to recieve a discount charge based on terms. Typically 1 to 3 years.  
Spot - bid for free compute capacity as it becomes available  
Dedicated Hosts - physical EC2 server dedicated for your use.  

Reserved - steady state or predictable usage
         - make upfront payments to receive discount
Spot - applications have flexible start and end times
     - applications only feasible at very low compute prices
     - users with urgent compute needs for large compute requirements
Dedicated Hosts - regulatory requirements
                - licensing reasons
                - can be discounted on long terms

Spot - if instance is terminated by Amazon for partial hour you will not be billed for that hour  
     - if instance is terminated by you for partial hour then you will be billed for that hour   

## EC2 Instance Types

D2 Dense Storage
R4 Memory Optimised
M4 General Purpose
C4 Compute Optimised
G2 Graphics Intensive
I2 High Speed Storage
F1 Field Programmable Gate Array
T2 Low Cost, General Purpose
P2 Graphics/General purpose GPU
X1 Memory Optimised

Anagram to remember different instance types:
    Dr Mc GIFT PX  

## EBS

Elastic Block Storage  

- Storage volumes attached to EC2 instances
- Block based storage so can run applications
- Placed in specific Availability Zone
- Automatically replicated within Availabilty Zone to prevent single component failure

### Types

- General Purpose SSD (GP2)  10,000 IOPS
- Provisioned IOPS SSD (IO1) More than 10,000 IOPS
- Throughput Optimised HDD (ST1) Frequently accessed
- Cold HDD (SC1) Less frequently accessed
- Magnetic (Standard) Standard, cheap and infrequently accessed


Cold HDD and Throughput Optimised HDD cannot be attached to Root volume  

By default when deleting EC2 instance the attached EBS volumes will be deleted also as 'Delete on Termination' option checked by default.  

** You cannot mount 1 EBS volume to multiple EC2 instances, consider EFS  

## Network Options 

- Automatically created Default VPC is default network
- One subnet equals one Availability Zone  

Security Groups are virtual firewalls that allow you to restrict access to EC2 instances on Protocol, Port, and Source IPs  

Key Pairs (public/private) are used to authorize access to EC2 instances  

### SSH to instance

- chmod 400 permissions set on key
- To login: ssh ec2-user@public_ip_address -i keyName.pem



