# Notes on DDL and Load Scripts

I wrote the original DDL scripts to be driven by the [Giraffle](https://optum.github.io/giraffle/#/) tools here:

https://github.com/dmccreary/tigergraph-clinical-lab/tree/master/db_scripts

These tools had the advantage that all the parameters of the load were centralized in a single properties file that can be reused in different environments (DEV, STAGE, TEST, PROD etc.).

Since these tools are not commonly used, we have now also provided a version of these scripts where the database name can be hard-coded.