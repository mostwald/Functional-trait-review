## Toward a functional trait approach to bee ecology

In review

[![DOI](https://zenodo.org/badge/719257598.svg)](https://zenodo.org/doi/10.5281/zenodo.10139286)

### Abstract

Functional traits are increasingly being used to predict species-level responses to environmental change. Trait data are abundant in the bee literature, yet we currently lack data standards for trait measurement and data sharing, hindering data reuse that could reveal large-scale patterns in bee functional ecology. Here, we present a roadmap toward community data standards for trait-based research on bees, including a protocol for interoperable trait data sharing. We also review the state of bee functional trait research across 97 studies, highlighting common measurement approaches and knowledge gaps in bee functional ecology. These studies were overwhelmingly situated in agroecosystems and focused predominantly on morphological and behavioral traits, especially body size, nesting biology, diet breadth, and sociality. Phenological traits were infrequently measured and physiological traits were nearly absent from our dataset. Studies investigating climate change effects were also rare. Along with our review, we present an aggregated morphological trait dataset compiled from our focal studies, representing 1209 bee species globally and serving as a template for standardized bee trait data presentation. We highlight obstacles to harmonizing this trait data, especially ambiguity in trait classes, methodology, and sampling metadata. Our framework for trait data sharing leverages common data standards to resolve these ambiguities and ensure interoperability between datasets, promoting accessibility and usability of trait data to advance bee ecological research. 

### Contents

* **Supplementary Table 1**
  Summarized information on functional traits commonly measured in bee ecological studies, with their functional significance, common methods of measurement in bee studies, and common states for traits involving categorical data. We additionally highlight traits that have been infrequently measured in functional trait studies (e.g., desiccation resistance, thermal tolerance, coloration), but which merit further attention due to their relevance to bee fitness and ecological interactions.

* **Supplementary Table 2**
  Metadata from 97 studies analyzed in our review, including citations, the traits analyzed, the types of trait measurements, and the data sources.
  
* **Supplementary Table 3**
  Trait classes, definitions, and associated data sources, where available, for the three most commonly studied behavioral traits: nesting biology, sociality, and diet breadth.

* **Supplementary Table 4**
  Harmonized primary morphological data compiled from our focal studies (see "Guide to the Morphological Dataset and the Data Upload Template" for metadata).

* **Supplementary Table 5**
  Template for standardized presentation of trait data. Column headers described below (see "Guide to the Morphological Dataset and the Data Upload Template).


### Guide to the Morphological Trait Dataset and the Data Upload Template

Below are definitions of the columns used in the trait dataset and template (Supplementary Tables 4 and 5). Where they correspond with the Darwin Core Standard (https://dwc.tdwg.org) they are mapped to those classes. 

#### Reference data

* **associatedReferences**: [DWC:associatedReferences](http://rs.tdwg.org/dwc/terms/associatedReferences) The literature reference associated with the trait measurement.
* **associatedReferencesID**: The global unique identifier (DOI) for the associated reference.


#### Taxonomic data

* **acceptedNameUsage**: [DWC:acceptedNameUsage](http://rs.tdwg.org/dwc/terms/acceptedNameUsage) The full name, with authorship and date information if known, of the currently valid taxon, e.g., ```Xylocopa sonorina Smith, 1874```. In this dataset, we have included the verbatim name as indicated by the studies' authors. Here, we have reported taxonomic names verbatim from their associated publications, so they do not all contain complete taxonomic information.
* **acceptedNameUsageID**: [DWC:acceptedNameUsageID](http://rs.tdwg.org/dwc/terms/acceptedNameUsageID) An identifier for the name usage (documented meaning of the name according to a source) of the currently valid taxon, e.g., ```gbif:1335321```.


#### Trait measurement data

* **traitName**: The relevant functional trait, e.g., ```body size```, ```tongue size```, ```pilosity```, etc.
* **measurementType**: [DWC:measurementType](http://rs.tdwg.org/dwc/terms/measurementType) The nature of the measurement, fact, characteristic, or assertion, e.g., ```body mass```, ```hair length```.
* **measurementTypeID**: An identifier for the measurement type. Here, we have linked to identifiers in the Hymenoptera Anatomy Ontology (http://portal.hymao.org/projects/32/public/ontology/), though other ontologies may be appropriate for other traits.
* **measurementMethod**: [DWC:measurementMethod]((http://rs.tdwg.org/dwc/terms/measurementMethod) A description or citation of the method or protocol used to determine the trait measurement.
* **measurementRemarks**: [DWC:measurementRemarks](http://rs.tdwg.org/dwc/terms/measurementRemarks) Comments or notes accompanying the measurement, e.g., ```right foreleg missing```.
* **recordLevel**: The biological level to which the measurement refers, e.g., ```individual```, ```species```, ```population```, or ```colony```.
* **measurementValue**: [DWC:measurementValue](http://rs.tdwg.org/dwc/terms/measurementValue) The value of the measurement, fact, characteristic, or assertion, e.g., ```45```, ```cavity nesting```, ```20.5```.
* **valueSummary**: The type of value or summary stastic represented by the measurementValue. This field specifies whether the value refers to measurements from to a single individual, e.g., "single observation", or data pooled from multiple individuals, e.g., ```mean```, ```median```.
* **measurementUnit**: [DWC:measurementUnit](http://rs.tdwg.org/dwc/terms/measurementUnit) The units associated with the dwc:measurementValue.
* **sampleSizeValue**: [DWC:sampleSizeValue](http://rs.tdwg.org/dwc/terms/sampleSizeValue) The number of individuals measured, if the measurementValue is a mean or other value pooled from multiple individuals.
* **variance**: A measure of variance in the measurement value, if applicable, typically for reported mean values.
* **varianceMeasure**: The type of value represented in the variance field, if applicable, e.g., ```standard deviation```,  ```standard error```.

#### Occurrence Data

* **recordNumber**: [DWC:recordNumber](http://rs.tdwg.org/dwc/terms/recordNumber) An identifier given to the occurrence at the time it was recorded. Often serves as a link between field notes and an occurrence record, such as a specimen collector's number, or an individual identifier assigned to a bee during an experiment. This identifier can link individual bees across trait datasets, when multiple functional traits are recorded for a single individual.
* **catalogNumber**: [DWC:catalogNumber](http://rs.tdwg.org/dwc/terms/catalogNumber) An identifier for the record within an established natural history collection.
* **verbatimEventDate**: [DWC:verbatimEventDate](http://rs.tdwg.org/dwc/terms/verbatimEventDate) The verbatim original representation of the date and time of specimen collection and/or measurement, e.g., ```summer 2017```, ```2022-02-08```.
* **eventDate**: [DWC:eventDate](http://rs.tdwg.org/dwc/terms/eventDate) The date-time or interval during which specimen collection and/or measurement occurred or was recorded. Recommended best practice is to use a date that conforms to ISO 8601-1:2019, e.g., ```2022-02-08```. We have reported event dates verbatim from the literature and have not converted them to ISO 8601-1:2019 format for this dataset, but recommend that future studies report data in this format.
* **sex**: [DWC:sex](http://rs.tdwg.org/dwc/terms/sex) The sex of the biological individual(s) represented in the measurement, e.g., ```male```,```female```,```hermaphrodite```,```males and females```.
* **lifeStage**: [DWC:lifeStage](http://rs.tdwg.org/dwc/terms/lifeStage) The age class or life stage at the time of occurrence/measurement, e.g., ```adult```,```egg```,```larva```,```pupa```.
* **locality**: [DWC:locality](http://rs.tdwg.org/dwc/terms/locality) The verbatim description of the place of occurrence, e.g., ```Bariloche```,```25 km NNE via Ruta Nacional 40 (=Ruta 237)```, ```Olympic National Park```.
* **verbatimLatitude**: [DWC:verbatimLatitude](http://rs.tdwg.org/dwc/terms/version/verbatimLatitude) The verbatim original latitude of the occurrence.
* **verbatimLongitude**: [DWC:verbatimLongitude](http://rs.tdwg.org/dwc/terms/version/verbatimLongitude) The verbatim original longitude of the occurrence.
* **decimalLatitude**: [DWC:decimalLatitude](http://rs.tdwg.org/dwc/terms/decimalLatitude) The geographic latitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of the location of the occurrence.
* **decimalLongitude**: [DWC:decimalLongitude](http://rs.tdwg.org/dwc/terms/version/decimalLongitude) The geographic longitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of the location of occurrence.
* **coordinateUncertaintyInMeters**: [DWC:coordinateUncertaintyInMeters](http://rs.tdwg.org/dwc/terms/coordinateUncertaintyInMeters) The horizontal distance (in meters) from the given decimalLatitude and decimalLongitude describing the smallest circle containing the whole of the location (real number). Leave the value empty if the uncertainty is unknown, cannot be estimated, or is not applicable (because there are no coordinates). Zero is not a valid value for this term.
* **country**: [DWC:country](http://rs.tdwg.org/dwc/terms/country) The name of the country or major administrative unit in which the location occurs.
* **stateProvince**: [DWC:stateProvince](http://rs.tdwg.org/dwc/terms/stateProvince) The name of the next smaller administrative region than country (state, province, canton, department, region, etc.) in which the location occurs.
* **county**: [DWC:county](http://rs.tdwg.org/dwc/terms/county) The full, unabbreviated name of the next smaller administrative region than stateProvince (county, shire, department, etc.) in which the location occurs.
* **habitat**: [DWC:habitat](http://rs.tdwg.org/dwc/terms/habitat) A category or description of the habitat of the location, e.g., ```oak savanna```, ```coastal sage scrub```.





## Citation
  
## Acknowledgements
We thank Istvan Miko for his support adding trait terms to the Hymenoptera Anatomy Ontology. This work was supported by three National Science Foundation (NSF) awards: DBI-2102006: Extending Anthophila research through image and trait digitization (Big-Bee) to KCS, DBI-2101851: Digitization TCN: Extending Anthophila research through image and trait digitization (Big-Bee) to VHG, and DBI-1560389: REU Site: Synergistic Studies of Honey Bees in the Republic of Turkey.

<a href="https://www.idigbio.org/wiki/index.php?title=TCN:_Extending_Anthophila_research_through_image_and_trait_digitization_(Big-Bee)&mobileaction=toggle_view_desktop"><img src="https://www.idigbio.org/wiki/images/8/84/Big-Bee-logo-2022.png" class="inline-image" style="height: 6em;"></a>
<a href="https://nsf.gov"><img src="https://big-bee.ccber.ucsb.edu/images/NSF_4-Color_bitmap_Logo-small.png" class="inline-image" style="height: 6em;"></a> 
