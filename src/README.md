# Notes on DDL and Load Scripts

I wrote the original DDL scripts to be driven by the [Giraffle](https://optum.github.io/giraffle/#/) tools here:

https://github.com/dmccreary/tigergraph-clinical-lab/tree/master/db_scripts

These tools had the advantage that all the parameters of the load were centralized in a single properties file that can be reused in different environments (DEV, STAGE, TEST, PROD etc.).  They had the disadvantage that the users needed to know a bit about configuring properties files and using the Gradle shell to run the scripts.

Since these tools are not commonly used, we have now also provided a version of these scripts where the database name can be hard-coded.  You will need to hand-edit the graph names if you don't use the default graph names.