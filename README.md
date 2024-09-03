# Task 1:  Data Validation UI with SHACL
## Background
SHACL is a RDF vocabulary and w3c recommendation for capturing data validation restrictions about RDF graphs. It is written in RDF and uses standardized terms to describe validation components such as cardinality, value ranges, object-property relationships etc. SHACL is essential in ensuring data quality in RDF datasets. Often, pipelines involving semantic data integration involve a crucial step of validating data before it is integrated. This step is often the responsibility of a domain-level expert checking the actual instance dataset against their mental image of what that data should look like. By translating that mental image into SHACL shapes allows for finding the instances in the dataset that do not conform to that mental image. Often, the result of such a SHACL shape validation will produce a report which should be used by a domain-level expert to improve the dataset (fix errors). This is the step which can be difficult, since profiency in RDF data, let alone SHACL shapes graphs, can be quite low. A user interface which improves the understandability and usability of SHACL (validation reports) would be very useful.

## Task
Front-end must be written in TypeScript, React, or other modern front-end language (no Python).

Write a small front-end which allows a user to upload an RDF data (in the lingo: an RDF graph). 

Create a functionality to “validate” the RDF data with the rules provided (in the lingo: RDF SHACL Shapes). You can use the SHACL API as back-end. We provide valid and invalid examples of RDF data.

The validation will return a “validation report” (also in RDF): use this report to best orient your user into correcting the RDF data.

Ensure a system for user friendly ability to upload, paste or drag file (contents), and for displaying the error(s) present in the RDF data. 

We will be looking at the user-friendliness, the design, and the fluidity of functionalities of your UI.

The users of your platform are familiar with RDF, but they are non-SHACL proficient user and non-coders.
