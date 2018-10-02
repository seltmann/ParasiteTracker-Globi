## Description of the content in vampire-moth-globi

[![Build Status](https://travis-ci.org/seltmann/vampire-moth-globi.svg)](https://travis-ci.org/seltmann/vampire-moth-globi)  [![GloBI](http://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:seltmann/vampire-moth-globi)](http://globalbioticinteractions.org/?accordingTo=globi:seltmann/vampire-moth-globi) 

[```Citation```](#Citation) / [```Interaction Types```](#interaction-types) / [```Data Definitions```](#data-definitions) / [```Included Resources```](#included-resources) /  [```Data Issues```](#data-issues) / [```Summary```](#summary)


### Description

vampire-moth-globi is a repository for interaction data about vampire moths and their fruit-piercing relatives (Lepidoptera: Erebidae: *Calyptra* spp.). The feeding observations are from the literature. A pdf of the original interpretation was put in a table format to include in presentations ([Zaspel, 2018](https://github.com/seltmann/vampire-moth-globi/blob/master/calyptra_hosts.pdf)).

This GitHub repository was cloned from [globalbioticinteractions/template-dataset](https://github.com/globalbioticinteractions/template-dataset), which includes a blank interactions.tsv, README and globi.json. GloBI requires that the interactions.tsv be called interactions.tsv and for the globi.json file to exist. Some column headers of inteteractions.tsv file was modified from the cloned template, but follow the naming conventions.

### Citation

Jennifer Zaspel. 2018. Biotic species interactions manually extracted from literature.


### Interaction Types

The biotic species interactions in this dataset were mapped to terms in the Relations Ontology (RO). Piercing was not available in RO, so ```biotically interacts with``` was used as a replacement.

interactionTypeName | interactionTypeId
--- | --- |
eats | http://purl.obolibrary.org/obo/RO_0002470
piercing | http://purl.obolibrary.org/obo/RO_0002437
enclosed conditions | http://purl.obolibrary.org/obo/ENVO_01001405
in nature | http://purl.obolibrary.org/obo/ENVO_01001226
under experimental conditions | http://purl.obolibrary.org/obo/ENVO_01001405
 
### Data Definitions

The definitions of the columns used in the interactions.tsv dataset are described here. If these correspond with Darwin Core they are mapped to those classes. Some of the columns in the template were unused.

  * A **InteractionID** : An non-unique identifier that links two interactions as part of the same observation in the dataset.
  * A **BasisOfRecord** [DWC:BasisOfRecord](http://rs.tdwg.org/dwc/terms/basisOfRecord) : The specific nature of the data record.
  * A **sourceTaxonId** [DWC:scientificNameID](http://rs.tdwg.org/dwc/terms/scientificNameID) : An identifier for the nomenclatural (not taxonomic) details of a scientific name.
  * A **sourceTaxonName** [DWC:scientificName](http://rs.tdwg.org/dwc/terms/scientificName) : The lowest level taxonomic rank that can be determined.
  * A **interactionTypeId** : Identifier for the interaction type.
  * A **isNegated** : This field is presently not supported in GloBI. It is intended to relate that a specific interaction was explicitly not observed.
  * A **interactionTypeName** : A interaction type (ex. eats, piercing). The name of the interaction type should be the name as it is listed in the original text, which is not always the name of the term it is mapped to. As long as the definition to the mapping is compatible with the ```interactionTypeName```, it is usable as a ```interactionTypeId```.
  * A **targetBodyPartName**  : The specific name of the target body part. The name of the body part should be the name as it is listed in the original text, which is not always the name of the term it is mapped to. As long as the definition to the mapping is compatible with the ```targetBodyPartName```, it is usable as a ```targetBodyPartId```.
  * A **targetBodyPartId**  : Identifer for the body part name.
  * A **experimentalConditionName**  : 
  * A **experimentalConditionId** : 
  * A **sexName** [DWC:sex](http://rs.tdwg.org/dwc/terms/sex) : The sex of the biological individual(s) represented in the Occurrence.
  * A **sexID**  : Identifer for the sex name.
  * A **targetTaxonId** [DWC:scientificNameID](http://rs.tdwg.org/dwc/terms/scientificNameID) : An identifier for the nomenclatural (not taxonomic) details of a scientific name.
  * A **targetTaxonName** [DWC:scientificName](http://rs.tdwg.org/dwc/terms/scientificName) : The lowest level taxonomic rank that can be determined.
  * A **targetCommonName** [DWC:vernacularName](http://rs.tdwg.org/dwc/terms/Taxon) : A common or vernacular name.
  * A **localityId** : Specific identifier for the locality. This field was not populated in this dataset.
  * A **localityName** [DWC:locality](http://rs.tdwg.org/dwc/terms/locality) : The specific description of the place. Less specific geographic information can be provided in other geographic terms (higherGeography, continent, country, stateProvince, county, municipality, waterBody, island, islandGroup). This term may contain information modified from the original to correct perceived errors or standardize the description. This field was not populated in this dataset. 
  * A **decimalLatitude** [DWC:decimalLatitude](http://rs.tdwg.org/dwc/terms/decimalLatitude) : 	The geographic latitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of a Location. Positive values are north of the Equator, negative values are south of it. Legal values lie between -90 and 90, inclusive. This field was not populated in this dataset.
  * A **decimalLongitude** [DWC:decimalLongitude](http://rs.tdwg.org/dwc/terms/decimalLongitude) : The geographic longitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of a Location. Positive values are east of the Greenwich Meridian, negative values are west of it. Legal values lie between -180 and 180, inclusive. This field was not populated in this dataset.
  * A **observationDateTime** [DWC:eventDate](http://rs.tdwg.org/dwc/terms/eventDate) : The date-time or interval during which an Event occurred. This field was not populated in this dataset.
  * A **referenceDoi** : This field was not populated in this dataset.
  * A **referenceCitation**  : The reference for the interaction.
  
### Included Resources

1. Bänziger, H. 1970. The piercing mechanism of the fruit piercing moth Calpe (Calyptra) thalictri Bkh. (Noctuidae) with reference to the skin-piercing blood-sucking moth Calpe eustrigata Hmps. Acta Tropica, 27: 54-88.
1. Bänziger, H. 1975. Skin-piercing blood-sucking moths I: Ecological and ethological studies on Calpeeustrigata (Lepid., Noctuidae). Acta tropica, (Basel) 32: 366-369.
1. Bänziger, H. 1979. Skin-piercing blood-sucking moths II: Studies on a further 3 adult Calyptra [Calpe] sp. (Lepid., Noctuidae). Acta Trop. 36(1):23-37.
1. Bänziger, H. 1986. Skin-piercing blood-sucking moths IV: Biological studies on adults of 4 Calyptra species and 2 subspecies (Lepidoptera, Noctuidae).Mittellungen der Schweizerischen Entomologischen Gesellschaft, 59: 111-138.
1. Bänziger, H. 1989. Skin-piercing blood-sucking moths V: Attacks on man by 5 Calyptra spp.(Lepidoptera: Noctuidae) in S. and S.E. Asia. Mittellungen der Schweizerischen Entomologischen Gesellschaft, 62: 215-233.
1. Bänziger, H. 2007. Skin-piercing blood-sucking moths VI: Fruit-piercing habits in Calyptra (Noctuidae) and notes on the feeding strategies of zoophilous and frugivorous adult Lepidoptera. Mittellungen der Schweizerischen Entomologischen Gesellschaft, 80: 271-288.
1. Quammen, D. Natural Acts: A Sidelong View of Science and Nature. 1985 pp. 47-52
1. Zaspel, J.M., V.S. Kononenko, and P.Z. Goldstein. 2007. Another blood feeder? Experimental feeding of a fruit-piercing moth on human blood in the Primorye Region of Far Eastern Russia (Noctuidae: Calpinae: Calpini). Journal of Insect Behavior, 20(5): 437-451.
1. Zaspel, J.M. 2018. Unpublished

### Data Issues

Several issues and decisions arose while translating the observations from the literature into a series of single observations. These issues are detailed in the [GitHub issues](https://github.com/seltmann/vampire-moth-globi/issues) for this project and also described here.

1. Not observed is presently not supported, but it can be included in the dataset.
1. A relationship in RO that specifically described the ```piercing``` is not available in RO, so ```biotically interacts with``` was used instead. Piercing may not imply eating.
1. Some of the interactions were observed under controlled conditions (e.g., in enclosed spaces) while in the field. These were interpreted as in an artificial or experimental environment even though they may have occurred outside.
1. *Ficus* is a homonym with a genus of sea snail. GloBI displays snail images for *Ficus* the fig. Better taxonomic concept resolution is much needed, not just in GloBI, but throughout our data systems.
1. There is presently not a way to depracate (or remove) a dataset from GloBI.


### Summary
The result is this dataset integrated with all other biotic interaction datasets. The interactions can be viewed on GloBI through the [interaction browser](https://www.globalbioticinteractions.org/browse/index.html?accordingTo=globi%3Aseltmann%2Fvampire-moth-globi&interactionType=interactsWith&resultType=json) or accessed through the [GloBI APIs](https://www.globalbioticinteractions.org/data.html).

![image of vampire-moth-globi](https://raw.githubusercontent.com/seltmann/vampire-moth-globi/master/network-bloodfeeding.png)(https://www.globalbioticinteractions.org/data.html)

