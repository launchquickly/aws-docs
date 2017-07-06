# CloudFormation

Scripted infrastructure

- Templates are in JSON Format
- Fields include Parameters, KeyName, DBName, DBUser, etc
- Outputs section can programatically be used to determine IP or DNS values for example
- Fn::GetAtt can be used to obtain an attribute value
- CloudFormation will rollback by default but this can be overriden in which case on error any created resources will not be deleted when an error is encountered



