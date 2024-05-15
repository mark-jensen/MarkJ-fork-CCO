# Common Core Ontologies
This repository contains the Common Core Ontologies (CCO), which comprise eleven interdependent ontologies containing classes and relations that serve as a mid-level reference for integrating data across any domain. CCO extends from the Basic Formal Ontology (BFO), a ISO standard top-level ontology [ISO/IEC 21838‑1](https://www.iso.org/standard/71954.html). BFO is [widely](https://basic-formal-ontology.org/users.html) used across the U.S. Government, the biomedical domain, and in industry. Both BFO and CCO have been endorsed by Chief Data Officers within the U.S. Department of Defense and Intelligence Community as baseline ontology standards.

TODO: add link to memo
TODO: list ontologies

CCO was created by [CUBRC Inc](https://www.cubrc.org/) under the direction of Ron Rudnicki around 2010. It was made open source in 2017. The Common Core Governance Board (CCGB) was founded in 2023 to ensure that CCO is maintained in perpetuity and independent of any particular individual, organization, or influence. 

TODO: Link to CCGB page

Founding members are: Mark Jensen, John Beverley, Alexander Cox, Neil Otte, and Barry Smith.

CCO is currently being standardized as [IEEE Standards Association](https://standards.ieee.org/develop/) [mid-level ontology](https://standards.ieee.org/ieee/3195/11025/). 

## Current Release 

* The current release of CCO is contained in CommonCoreOntologies.ttl and is located in this root directory. 
* The most current versions of these files that the release is built from can always be found at: https://github.com/CommonCoreOntology/CommonCoreOntologies/src/core.
* The files in the `master` branch will always be identical to the current release.
* Current user guides, best practices, and other documentation relevant to the current release can be found in /documentation.
* More information about CCO's release strategy can found [here](). TODO: add link

## Directory Structure

* src/
  - core: contains the eleven core ontologies plus an import interface AllCoreOntology.ttl.
  - import: contains bfo-core.ttl.
  - mro: contains the ModalRelationOntology.ttl.
  - code: contains queries and scripts used to build CCO.

* documentation/
  - ontology-diff-files: contains any diff files per ontology between the current release and previous release.
  - legacy-documentation: contains previous, potentially outdated, documentation. 


## CCO Ontologies
```mermaid
graph TB
    A(BFO):::BFO --> B(Information Content Entity):::CCO
    A(BFO) ---> C(Material Artifact):::CCO
    A(BFO) ---> D(Geospatial Region):::CCO
    A(BFO) ---> E(Organization):::CCO
    A(BFO) ---> E(Environmental Feature):::CCO
    C(Information Entity Ontology) --> F(Artifact Ontology):::CCO


classDef BFO fill:#F5AD27,color:#060606
classDef CCO fill:#277DF5,color:#060606