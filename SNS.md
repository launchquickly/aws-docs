# SNS

Simple Notification Service

Set up, operate and send notifications

- Follows the publish-subscribe (pub-sub) messaging paradigm
- Uses 'push' mechanism
- Topic based
- SMS text message or email
- To SQS or HTTP endpoint
- To mobile devices natively on Apple, Android etc

- Topic - access point to allow recipients to dynamically subscribe
- Formats delivered message dependent on client type
- Pay-as-you-go
- TTL if specified value exceeded message will expire 

- JSON data format amongst others
- Type, MessageId, TopicArn, Subject, Message, Timestamp, SignatureVersion, Signature, SigningCertURL, UnsubscribeURL, MessageAttributes fields

- Protocols include: HTTP, HTTPS, Email, Email-JSON, Amazon SQS, Application
