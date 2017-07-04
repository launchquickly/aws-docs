# SQS

Simple Queuing Service

- web service that gives you access to message queue
- distributed queue system
- queue is temporary repository for messages awaiting processing

- used to decouple components of an application

- messages can contain up to 256kb of text in any format
- billed at 64kb "Chunks"
- single request can have between 1 to 10 messages, up to a maximum total payload of 256kb

- First 1M requests p/m free
- $0.50 per milliion requests p/m
- Each 64kb 'Chunk' counts as 1 request

- queue acts as a buffer between producer and consumer
- useful where produce is producing work faster than consumer can process it or if either the producer or consumer are only intermittently connected to network

- delivery of message "at least once". e.g. duplicate checker or similar may be required
- supports multiple readers and writers interacting with the same queue
- highly available
- no ordering (FIFO) guarantee
- if ordering is important sequencing information should be placed in each message
- consumer had to pull message (not push)

- maxium retention period of a message is 14 days
- visibility timeout period starts once pull occurs
- if visibility timeout period expires the message will be available again in the queue
- default visibility timeout is 30 seconds
- maxium visibility timeout is 12 hours
- deletion from the queue indicates completion of processing of message

- messages can be delivered multiple times and in any order
- separate queues can be used by applications to indicate prioritisation
- ChangeMessageVisibility action can be used to specify a new visibility timeout value. Using the call restarts the clock to 0.
- Long polling doesnt return a response until a message arrives or the long poll times out
- Maxium Long Poll Time out = 20 seconds
- Long polling can reduce CPU cycles

Fanning out - SNS topics first using SNS then create and subscribe multiple SQS queues to SNS topic  



