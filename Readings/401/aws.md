# SNS VS SQS

## SNS
- Publisher / subscriber system 
- Publishing messages to a topic can deliver to many subscribers of different types.

do OTHER SYSTEMS care about an event?
SNS is the broadcast messages
## SQS

- queueing service for message proceessing 
- a system must polll the queue to discover new events
- MEssafes in the queue are typically processed by a single consumer

does YOUR SYSTEM care about an event?
if a message gets delivered to the SQS it is gurenteed to be saved. LLamda will not save this message.

## why???

we want to decouple the stages of our events. IF we were to run all of these events in sequence of eachother it would take a very long time and we would get outlier cases like charging the customer twice bevause the logic in the analytics SQS failed. Decoupling these events keeps our code more secure, and functioning as intended,
