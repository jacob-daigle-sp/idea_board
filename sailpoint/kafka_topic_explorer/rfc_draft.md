- Feature Name: Kafka Topic Explorer
- Start Date: 2020-06-15
- RFC PR: 
- JIRA Issue: 

# Summary
[summary]: #summary

This RFC proposes an outline of new features for our existing Chronicle Service that will introduce new ways of interacting with and exploring kafka.

Features:
* Explore available kafka topics and understand their use case/creation
* Export limited kafka messages
* Understand producers and consumers of a given topic and given events in topics
* Understand and update topic schemas
* Inspect metrics around consumer and consumer group offsets as requested


# Motivation
[motivation]: #motivation

This feature is a potential tool to accelerate our usage of kafka. As stream based systems get adopted it will become critical to understand what topics and tables we have, why they were created, who is consuming from them, and simplistic ways to pull data from them. 

Motivating examples for the above features may be:
- A developer is looking for data xyz, rather than reaching out to many teams, they can search topics via the explorer.
- A developer needs to understand what type of data flows though a topic. Sure a dev can spin up a console consumer, but as we adopt different sterilization (I advise avro) pulling messages via a console consumer gets cumbersome.
- A developer wants to understand upstream dependencies of a given data stream
- A developer wants to tear down a stream, and needs to know who is consuming the data down stream
- Dev ops needs to monitor lag of given application not producing metrics

# Guide-level explanation
[guide-level-explanation]: #guide-level-explanation


# Reference-level explanation
[reference-level-explanation]: #reference-level-explanation


# Drawbacks
[drawbacks]: #drawbacks

Chronicle would only host a subset of features, we may end up building another tool later which would complement the abilities granted to Chronicle. These extra features may include self service to spin up topics in non prod enviornments.

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

Alternatives to this could be a guru page listing data dependencies, which will fall out of date. 

For easy of use in developmental purposes, having devs download something like [Kafka Magic](https://www.kafkamagic.com/) or [Kafka Tool](https://www.kafkatool.com/) which could be viewed as a security issue.

 
Another alternatives is just to host our own version of kafka tool or kafka magic. It looks like we have deployed something similar here [here](http://kafka-m-820325191.us-east-1.elb.amazonaws.com/clusters/us-east-1-dev/topics/).  

# Prior art
[prior-art]: #prior-art

Nothing built in sailpoint, but inspiration can be pulled from the following:
* [Kafka Magic](https://www.kafkamagic.com/)
* [Kafka Tool](https://www.kafkatool.com/)


# Unresolved questions
[unresolved-questions]: #unresolved-questions

- Who would own this? 

# Future possibilities
[future-possibilities]: #future-possibilities

Self service to create topics and mirror makers.