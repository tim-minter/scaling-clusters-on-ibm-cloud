# scaling-clusters-on-ibm-cloud

One advantage of cloud is that costs should be lower than owning your own hardware. That is pretty much automatic, but there is a lot more you can do to fine tune costs, particularly in your developement environment. 
In non cloud world, you wouldn't really want to turn off your physical servers each night but in Cloud this is very much a possibilty, and to save costs and general power usage for the world, it might be the best idea.

In IBM Cloud there are several ways to turn off a virtual server when it's not being used, and not all of them suspend billing. Note also that billing for storage will still carry on unless you delete that of course.

1. Go into the operating system and power it down manually - this doesn't suspend billing
2. Call the Cloud Foundry API to issue a shutdown - billing is suspended
3. Issue the ibmcloud sl vs power-off command from a scheduled task or manually - billing is suspended
4. Via an autoscheduling service - billing is suspended

The server you are powering down also has to be one that is billed hourly (not monthly) and be one of the standard t-shirt sizes. this document explains what servers are elegible for billing suspension https://cloud.ibm.com/docs/virtual-servers?topic=virtual-servers-requirements

[in progress]

Thank you to Philippe THOMAS for my questions about this
