# resource-gtfs-bench-rml

This repository contains a Maven project setup for RDFizing GTFS data.

The process relies on the [rpt-maven-plugin](https://github.com/Scaseco/rpt-maven-plugin).

* Source Data:
  * [data/csv/1](data/csv/1) contains the GTFS ZIP archive [gtfsbench-csv-1.zip](data/csv/1/gtfsbench-csv-1.zip) together with a Maven packaging. Running `mvn install` installs the package into the local repository.

* Mapping:
  * [mapping](mapping) contains packaging of an RML mapping as a Maven artifact. Running `mvn install` installs the package into the local repository.

* Mapping Execution / RDF Generation
  * The folder [rdfize](rdfize) contains a Maven project that declares dependencies on the source data and the mapping. Running `mvn install` executes the mapping and install the result into the local repository. Running `mvn install` produces the RDF output.



