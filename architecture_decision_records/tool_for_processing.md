**Title**

ADR Ad Click Stream Platform: Processing Tool

**Context** 
This processing tool would be used to process the raw data and transform it (deduplicate, cleanse) to silver layer and also to transform it to create the KPIs for gold layer.

**Decision** 

Decided to choose Apache Flink for processing. 

**Status** 

Active

**Trade-offs**
- Spark vs Flink: Pyspark streaming is another option but can only achieve micro-batch processing. Whereas, Flink can do real-time streaming. 
- Since latency is an important constraint in this use case I chose Flink.

**Consequences** 
- Flink is not as easy to develop compared to Spark code, which Python APIs on top of it.
