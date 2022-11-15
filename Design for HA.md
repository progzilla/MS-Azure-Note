# DESIGN FOR HA

<b>1. Identify HA Requirement</b>

HA workloads are:
- Resilient to component failure
- Can run in a healthy state with no significant downtime

- HA Targets<br />
-- consider cost & complexity(define SLA)<br />
--- self-healing & self-diagnosing<br />
--- detecting outages quickly<br />
--- define tolerable time window<br />
--- consider MTBF & MTTR measurements.<br />
-- Identify Dependencies<br />
--- internal and external dep.<br />
--- esp. external deps must be HA<br />
--- Identify critical system flows<br />
--- Identify less critical components<br />
- Availability Metrics<br />
-- MTTR(avg. time to restore)<br />
-- MTBF(how long a component outage is reasonably expected to last)<br />
- Understand SLAs<br />
-- its all about Micrsoft's commitment to uptime & connectivity<br />
-- Different services have diff. SLAs<br />
-- if SLA isn't met, some service credit is issued to the customer<br />
-- SLAs acts as enforcement policy<br />
-- Use SLA estimator<br />


<b>2. Azure Front Door</b>




<b>3. Azure Traffic Manager</b>

<b>4. HA Solution for Compute</b>

<b>5. HA Solution for SQL</b>

<b>6. HA Solution for Non-SQL</b>

