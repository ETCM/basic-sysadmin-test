Disaster Recovery Design and Verification
=========================================
Answer the following questions immediately below each question.

Q1) Disaster Recovery and Continuous Operations
-----------------------------------------------
What is the relationship between DR and COOP? What are the driving factors
pertaining to this type of planning?

Both DR and COOP need to be built in to an organization's business continuity planning. While disaster recovery is a huge part of an organization response to adverse conditions they also need to make sure that the safeguards and measures for ensuring that vital systems stay online. COOP needs to take in to account that certain portions of the infrastructure need to be functional at all times so that the DR plan can be optimally implemented in the event a disaster occurs. The COOP plan needs to fully support the DR plan.

The factors that should drive these programs are the maximum allowable time critical systems can be down, what systems can't afford to be down at all, any relevant service level agreements the organization must maintain and what systems need to be restored to operation first.

Q2) Disaster Recovery Planning
------------------------------
How do DNS, layer-4 switches and layer-7 logic relate to DR situations? What
is a transparent failure?

During the disaster recovery phase systems must be returned to operational status in an acceptable amount of time. DNS can play a part in this both internally and externally. Internally, any DNS servers that are down can cause internal resource resolutions issues. Applications may cease to function if they can not resolve any hostnames that may be held on servers that are not functional. Externally, it must be determined when Internet service will be restored. If there is a failover is improperly configured or non-existent then external records may need to be changed to point to alternative sites or a backup provider to ensure external facing resolution can still take place.

A layer-4 switch could be key to a DR plan because it allows the load balancing function to be configured for failover. In the event a disaster were to occur, a layer 4 switch could potentially keep the network functioning off another service providers network.

Layer-7 logic is critical to restoring business functions on critical applications. Without the presence of this logic a company cannot perform the majority of it's duties.

Transparent failure refers to a situation in which a device fails but it is not noticed by end user because the failover system takes over services without interruption. This is a great asset within a disaster recovery scenario since critical systems can continue to stay operational and downtime is non existent.

Q3) Disaster Recovery Practice
------------------------------
How does production deployment relate to DR? Describe the concerns with
reverting a production deployment.

A production deployment should take your DR plan in to consideration since the success of recovering from a disaster relies heavily on the proper deployment processes being in place. This could include items such as taking a full backup of the initial system, making sure redundant power supplies are in use and making sure equipment is placed on some sort of backup power supply.

When a production deployment is reverted, factors such as cost of lost productivity and lost labor must be considered. The amount of data between the time or reversion and the last backup also come in to consideration.

Q4) DR Scenario
---------------
You have a production site with a partial service-capacity, replicated back-up
site. The primary and back-up sites are connected with a direct fiber backplane
for fail-over and consistency communication. Someone hits the fiber with a
backhoe. Is this an issue? If it is, how would you design the total system to
mitigate any problems?

I believe this would be a problem since fiber is a fragile medium. In order to mitigate issues like this, proper placement of cabling, construction and maintenance guidelines and redundant cabling would need to be implemented.
