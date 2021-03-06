# [rs.gbif.org](http://rs.gbif.org)
GBIF **R**epository of **S**chemas hosted at http://rs.gbif.org

## Deploying
Deploying this is through a git pull and then running the script to build the extension inventory files:
```
  rs.gbif.org /var/www/rs.gbif.org $ sudo git pull
  rs.gbif.org /var/www/rs.gbif.org $ sudo ./sync-extensions.py
```
This happens automatically by a cron job running on the server hosting `rs.gbif.org`.

## Darwin Core Archive extensions and vocabularies
The folder [core](core) contains [IPT](https://www.gbif.org/ipt) XML definitions for [Darwin Core Archive](http://rs.tdwg.org/dwc/terms/guides/text/) core data files. [Production extensions](extension) and associated [vocabularies](vocabulary) are hosted here, as well as [sandbox](sandbox) definitions of those used by IPT test installations.

Instructions for how to create new versions of extensions and vocabularies can be found [here](versioning.md).

## Named Area Standards
The folder [areas](areas) lists geographic area standards and recommends a namespace prefix for each of them to be used as part of the [dwc:locationID](http://rs.tdwg.org/dwc/terms/locationID) in particular inside the [GNA Species Distribution Extension](http://rs.gbif.org/extension/gbif/1.0/distribution.xml)

## Conventions
Coding conventions and styles for IntelliJ and Eclipse.

## Dictionaries
Dictionaries for name parsing and finding.

## Schemas
XML schemas for extensions, vocabularies, EML, Dublin Core, etc.

## Templates
Crawling templates for DiGIR and BioCASe.

## Terms
Term definitions in RDF, including Darwin Core Term definitions translated into various languages.
