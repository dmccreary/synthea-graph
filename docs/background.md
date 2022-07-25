# Background

This document describes the historical background for how we made a decision to open source these benchmarks.

## 2017: Database Vendor Benchmarking

In 2017 Optum was going through a process of benchmarking various graph databases.  We found that we needed a consistent way to evaluate the pros and cons of each database software system.  We developed a set of benchmarks using the [Synthea](https://synthetichealth.github.io/synthea/) synthetic clinical data generation system.  We developed a simple labeled property graph [model] and then loaded 10 million synthetic patients into this model running on various vendor databases.  After the data was loaded we then performed various stress tests on the system to see what the limits of each software system was.

## 2020" Hardware Benchmarking

In 2020 we also found that these same benchmarks were ideal to compare different hardware systems.  We worked with both TigerGraph and Dell's Healthcare division to create a state-of-the-art hardware system that is custom tuned to perform large graph queries that are distributed over a 8-node cluster.

This paper:

[Dell TigerGraph Case Study](https://github.com/dmccreary/synthea-graph/blob/main/resources/Dell-TigerGraph-Case-Study-Optum.pdf)

is a result of this analysis.  Note that this paper found that we could retrieve a full patient record from a group of 11M patients in an incredible 8.5 milliseconds.  This was roughly 10x faster than many of our production systems at the time.  This incredible result could not have been done without the careful configuration and tuning of the 128-core EPYC hardware and the dedication of the engineers from both TigerGraph and Dell working together over a period of six months.

## 2022: Optum Open Sources Benchmarks

Now in 2022, with the partnership of the [Optum Office of Open Source](https://opensource.optum.com/), we are making these benchmarks available to the public using a liberal open source license.  This means that any software vendor can also use these benchmarks to see how their systems hold up under the stress of real-world clinical analytics workloads.

We hope everyone finds these benchmarks useful at helping us all lower the cost of healthcare for everyone.