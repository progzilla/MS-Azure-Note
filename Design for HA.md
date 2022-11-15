# DESIGN FOR HA

<b>Identify HA Requirement</b>

HA workloads are:
- Resilient to component failure
- Can run in a healthy state with no significant downtime

- HA Targets
-- consider cost & complexity(define SLA)
--- self-healing & self-diagnosing
--- detecting outages quickly
--- define tolerable time window
--- consider MTBF & MTTR measurements.
-- Identify Dependencies
-- internal and external dep.
-- esp. external deps must be HA
-- Identify critical system flows
-- Identify less critical components
- Availability Metrics
-- MTTR(avg. time to restore)
-- MTBF(how long a component outage is reasonably expected to last)
- Understand SLAs
-- its all about Micrsoft's commitment to uptime & connectivity
-- Different services have diff. SLAs
-- if SLA isn't met, some service credit is issued to the customer
-- SLAs acts as enforcement policy
-- Use SLA estimator


<b>Azure Front Door</b>



<b>Azure Traffic Manager</b>

<b>HA Solution for Compute</b>

<b>HA Solution for SQL</b>

<b>HA Solution for Non-SQL</b>

Service Tiers: DTU & vCore

