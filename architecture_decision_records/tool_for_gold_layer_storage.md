**Title**

ADR Ad Click Stream Platform: Gold layer storage

**Context** 

This layer would contain the key metrics needed in the internal dashboard.

**Decision** 

To use AWS Athena for Gold layer storage

**Status** 

Active

**Consequences** 

- OLAP data storage solution --> better for aggregations and transforming and storing metrics
- Has features such as cataloging --> for governance and lineage
- Can build a semantic layer on top of it --> would help business users to understand the key metrics and business terms.
