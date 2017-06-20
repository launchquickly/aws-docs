# IAM

Identify Access Management

Allows you to manage users and their level of access  

- Centralised control of AWS account  
- Shared access to your AWS account  
- Granular Permissions  
- Identify Federation - including Active Directory, LinkedIn, etc  
- Multifactor Authentication  
- Provide temporary access for users/devices where necessary  
- Set up your own password and rotation policy  
- Integrates with many different AWS services  
- Supports PCI DSS Compliance  

- IAM is universal it is not region specific  
- 'root account' created when you first set-up AWS has complete Admin access  
- New users have NO permissions when first created  
- AWS credentials (access key & secret access key) are generated once and are non-recoverable  
- Always setup MFA on your 'root account'  

Users - people  
Groups - collections of users under one set of permissions, where permissions are derived from policies  
Roles - assign them to AWS resources  
Policy Documents - document that defines one or more   permissions that are attached to users, groups or roles  
            - defined in JSON

** User can use Access Key ID & Secret access key to programatically interact with AWS services  

User use Username and password to login to console  

Permissions can be attached directly to a user independent of Groups or Roles  

## ADFS
- can be used to authenticate via SAML  
- always authenticte against ADFS first then you are assigned temporary security credential  

## Web Identity Federation with Mobile Applications
- you can use Facebook, Google, Amazon, etc to authenticate with  
- this is done via access token which provides temporary security credentials (AssumRoleWithWebIdentity request)  
- see [STS](/STS.md) for choreography




