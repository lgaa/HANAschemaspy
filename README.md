# HANA plugin for SchemSpy
http://sourceforge.net/projects/schemaspy/

## Usage
## 1. Rebuild SchemaSpy

place `hana.properties` inside schemaspy path `/src/main/resources/net/sourceforge/schemaspy/dbTypes/` and rebuild the jar

## 2. Use via commandline switch

schemaspy supports the `-t` parameter, where you can either list the database type to use (pulling from the schemaspy jar) or specify the `hana.properties` file directly.

## Common Remarks
Please make sure you use the right port number, it is computed from the HANA databases instance number.

The formula is: `30015 + ( InstanceNumber * 100 )`.
Example: Instance 42: `30015 + ( 42 * 100 ) = 34215`
