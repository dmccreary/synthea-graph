# References

## Dell-TigerGraph 2020 Clinical Benchmark

[Graph Analytics in Healthcare Operations: A case study of TigerGraph on Dell EMC Infrastructure]
([Dell TigerGraph Case Study](https://github.com/dmccreary/synthea-graph/blob/main/resources/Dell-TigerGraph-Case-Study-Optum.pdf))

## Synthetic Data Vault

Our baseline clinical data leverages the power of generating patient-by-patient data based on real-life examples of conditions.

If you have actual clinical data and you want to use this data to generate your own clinical data, we recommend using a tool such as the [Synthetic Data Vault](https://sdv.dev/) to generate a sample of data.  SVD does a good job at generating flat tabular data with CSV files.  It is not strong at generating structure and relationships that we find in actual clinical graphs.

## MIMIC-III

MIMIC-III is a large, freely-available database comprising deidentified health-related data associated with over 40,000 patients who stayed in critical care units of the Beth Israel Deaconess Medical Center between 2001 and 2012.  This dataset is too small for us to use for benchmarking large distributed graphs, but we can use MIMIC-III to train synthetic generation tools.

[MIMIC-III](https://physionet.org/content/mimiciii-demo/1.4/)
