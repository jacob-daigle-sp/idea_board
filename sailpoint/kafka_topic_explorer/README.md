- Feature Name: `kafka_topic_explorer`
- Start Date: na
- RFC PR: na
- JIRA Issue: na

# Summary
[summary]: #summary

This document proposes the creation of a new engineering tool, the Kafka Topic Explorer. This tool will be a self service tool for developers to:
* create and configure kafka topics
* create and configure and mirror makers
* explore available kafka topics and understand their use case/creation
* export limited kafka messages
* understand producers and consumers of events published to different topics
* understand topic schemas
* inspect consumer and consumer group offsets

Examples:
    
* [Kafka Magic](https://www.kafkamagic.com/)
* [Kafka Tool](https://www.kafkatool.com/)
    

# Motivation
[motivation]: #motivation`

The primary motivations for this proposal are to resolve the inefficiency with interacting with kafka. As it stands today, developers are not able to easily to create topics, nor have no way of understanding what topics currently exist and what the data within looks like. 

Further to the above points, in the event production systems are locked down, we could use the above described tool to serve as a request/management system for kafka topics to be created.

# Guide-level explanation
[guide-level-explanation]: #guide-level-explanation


# Reference-level explanation
[reference-level-explanation]: #reference-level-explanation


# Drawbacks
[drawbacks]: #drawbacks

- No real draw backs here, this will take some engineering effort, but will allow the engineers to move faster. 

# Rationale and alternatives
[rationale-and-alternatives]: #rationale-and-alternatives

-

# Prior art
[prior-art]: #prior-art

- Currently we have an dev ops system in place to create kafka topics based on email requests. 


# Unresolved questions
[unresolved-questions]: #unresolved-questions

- 

# Future possibilities
[future-possibilities]: #future-possibilities

-