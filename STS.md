# STS

Security Token Service

Grants users limited and temporary access to AWS resources from one of 3 sources:

- Federation e.g. Active Directory
- Federation with Mobile Apps e.g. OpenID provider
- Cross Account Access e.g. across AWS accounts

Identity Broker - join identity from one source to another e.g. IAM to Active Directory  

Identity Source - IAM, Facebook, Active Directory, etc  

## User Scenario

1. Enter username & password
2. Call Identity Broker
3. Identify Broker uses organisations LDAP to validate employee's identity
4. Identity Broker calls GetFederationToken via IAM credentials. Call includes IAM policy, duration, policy specifying premissions to be granted temporarily
5. STS confirms policy of IAM user making call and returns 4 values: access key, secret access key, token, and a duration
6. Identity Broker returns temporary security credentials to application
7. Data storage application uses temp credentials to make request to S3
8. S3 uses IAM to verify request via temporary credentials


## Role Scenario
- similar to previous scenario but Role used in place of User Id  


