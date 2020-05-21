- Feature Name: `kafka_topic_explorer`
- Start Date: na
- RFC PR: na
- JIRA Issue: na

# Summary
[summary]: #summary

This RFC proposes the creation of a new engineering tool, the Kafka Topic Explorer. This tool will be a self service tool for developers to:
* create kafka topics and mirror makers
* configure kafka topics and mirror makers
* explore kakfa topic messages
* explore different kafka topics/tables
* understand producers and consumers of events published to different topics


# Motivation
[motivation]: #motivation`

The primary motivations for this proposal are to resolve the inefficiency with interacting with kafka. As it stands today, developers are not able to easily to create topics, further to that point, developers have no way of understanding what topics currently exist and what the data within looks like. 

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