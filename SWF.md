# SWF

Simple Workflow Service

Webserice that coordinates worka across distributed application components. Enables applications to be designed as a coordination of tasks.

- Workers are programs that interact with SWF to get tasks, process tassk and return results
- Decider is a program that controls the coordinations of tasks - i.e. their ordering, concurrency and scheduling logic
- SWF is the broker of interactions between Workers and Deciders
- Ensures tasks is assinged only once and is never duplicated
- SWF maintains applications state durably so that Workers and Deciders don't have to keep track of execution state
- Workflow and activity type are scoped to a domain
- Domains isolate a set of types, executions, and task lists form others within the same account.
- JSON format used to specifiy parameters of SWF Domains
- Maximum Workflow can be 1 year and value measured in seconds


- SWF task-orientated vs SQS message orientated
- SWF ensures taks assigned only once, SQS you have to handle duplicated messages and processing only once
- SWF keeps track of all the tasks and events in an application

