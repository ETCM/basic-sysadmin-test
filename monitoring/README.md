Production Monitoring
=====================

Q1) A service is repeatedly crashing. How do you identify possible causes?
--------------------------------------------------------------------------
Using the dmesg | grep combined command should be helpful in allowing me to find any issues that may have occurred in the kernal. Checking the information in the logs of the service that crashed would also be a good start.

Q2) Scenario:
-------------
Given a collection of internal assets which are partitioned into several classes where each class runs a distinct set of services. Network structure is such that two nodes of different classes may not be able to directly communicate. One class of nodes is for data aggregation and another integrates to an external enterprise peer. There is a message bus for passing work between classes.

Describe in bullet points how you would monitor such a system. Include a set of health metrics and targets.

- Install programs such as Nagios and Nagios Fusion for monitoring of these systems
- Monitor access requests from restricted targets
- Monitor network connectivity and service heartbeats
- Monitor connectivity to the enterprise peer
- Monitor the critical services and notify appropriate parties if services go down

Q3) In Linux, how do you identify what resources a given process has?
---------------------------------------------------------------------
Using ps aux should show the associated resources and processes.

