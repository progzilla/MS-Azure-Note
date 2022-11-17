# DESIGN FOR HA

<b>1. Identify HA Requirement</b>

HA workloads are:
- Resilient to component failure
- Can run in a healthy state with no significant downtime

- HA Targets<br />
	- Consider cost & complexity(define SLA)<br />
		- self-healing & self-diagnosing<br />
		- detecting outages quickly<br />
		- define tolerable time window<br />
		- consider MTBF & MTTR measurements.<br />
	- Identify Dependencies<br />
		- internal and external dep.<br />
		- esp. external deps must be HA<br />
		- identify critical system flows<br />
		- identify less critical components<br />
- Availability Metrics<br />
	- MTTR(avg. time to restore)<br />
	- MTBF(how long a component outage is reasonably expected to last)<br />
- Understand SLAs<br />
	- Its all about Micrsoft's commitment to uptime & connectivity<br />
	- Different services have diff. SLAs<br />
	- If SLA isn't met, some service credit is issued to the customer<br />
	- SLAs acts as enforcement policy<br />
	- Use SLA estimator<br />


<b>2. Azure Front Door</b>

A modern CDN/AppDN using Microsft's Edge Network

- Optimizes access to content
- Providers another layer of reliability
- Offers intelligent threat protection
- Provides Global LB & site Acceleration for WebApp
- Offers 7 layer 7 capabilities e.g 
	- SSl offload, 
	- path-based routing, 
	- fast failover,
	- caching, etc

Case Study - FD for Reliability

![Azure Front Door Use Case](https://learn.microsoft.com/en-gb/training/wwl-azure/design-for-high-availability/media/front-door-integrate.png "Azure Front Door Use Case")

 - The use of priority-based routing for traffic
 - For HA, a secondary region serves is on standby for failover
 - Geo-replication is used to sync data to stanby region
 
HA Approaches

 - A/P+HS: HS means VMs in s*by region are on AlwaysOn mode. Expensive
 - A/P+CS: CS means VMs in s*by region aren't allocated till needed for failover. Cheaper but not so reliable
 - A/A: Both regions are active with LB serving requests btw them.


<b>3. Azure Traffic Manager</b>



<b>4. HA Solution for Compute</b>

<b>5. HA Solution for SQL</b>

<b>6. HA Solution for Non-SQL</b>

