# Synthea To Graph

This site will allow you to generate large clinical datasets and load them to a graph database.  This project is ideal if you are benchmarking clinical algorithms and testing your clinical machine-learning algorithms at scale.

The microsite for this repository is here:

    [http://dmccreary.github.io/synthea-graph](http://dmccreary.github.io/synthea-graph)

## Background

[Synthea](https://synthetichealth.github.io/synthea/) is a tool for generating synthetic healthcare records.  The current version generates a patient record and related clinical information such as allergies, claims, diagnosis, prescriptions, vaccinations, etc.  You can generate any arbitrary-sized patient population, you are only limited by the disk space on your servers.

A typical use is the following command:

$ synthea_run -p 10000

Which will generate 10 thousand sample patient records.  The default format is FHIR, but we find that changing the config files to generate CSV files is more efficient.

After the files are generated, you can use the tools in this repository to load this data into TigerGraph.

## Once you have generated t

## Mkdocs

This site is built with the mkdocs system.

### Mkdocs Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
