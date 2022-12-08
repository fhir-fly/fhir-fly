# FhirFly FHIR Server

## Purpose
The purpose of this project is to build a cloud native and reactive FHIR Server using Quarkus 
and Mutiny. It should not only support `application/fhir+xml` and `application/fhir+json` data 
formats, but also `application/fhir+turtle` using a triple store. 

The FHIR Server should support multiple backend storage types and vendors, including 
(but not limited to):

- JPA (Postgres)
- RDF4J (GraphDB)
