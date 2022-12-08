# FhirFly - Bill of Material

## Purpose
Defines the Maven bill of material of the project, meaning that it is a pom containing a 
dependency management section with all dependencies used in this project. This includes all 
modules produced by this project as well.

If you want to use artifacts of this project in your own project, for example to build your
own FHIR Server, you can do so by importing this bill of material into your project as 
following:

```xml
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>io.fhirfly</groupId>
            <artifactId>fhirfly-bom</artifactId>
            <version>1.0-SNAPSHOT</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
    </dependencies>
</dependencyManagement>
```
The pom should NOT contain FhirFly build specific dependencies, plugins, etcetera, as we don't 
want to force any of our build requirements on the users of this pom.
