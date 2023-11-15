## Toward a functional trait approach to bee ecology

[Madeleine M. Ostwald](https://orcid.org/0000-0002-9869-8835), [Victor H. Gonzalez](https://orcid.org/0000-0002-4146-1634), Carrie Chang, Nydia Vitale, [Mariano Lucia](https://orcid.org/0000-0001-8019-6768), [Katja C. Seltmann](https://orcid.org/0000-0001-5354-6048)

In review

[![DOI](https://zenodo.org/badge/719257598.svg)](https://zenodo.org/doi/10.5281/zenodo.10139286)

### Abstract

Bee functional traits are increasingly being used to predict species-level responses to environmental change. Trait data are abundant in the bee literature, yet we currently lack data standards for trait measurement and data sharing, hindering opportunities for meta-analyses that could reveal large-scale patterns in bee functional ecology. Here, we analyze the state of bee functional trait research across 97 studies, reviewing common trait measurement approaches and knowledge gaps in bee functional ecology. These studies were overwhelmingly situated in agroecosystems and focused predominantly on morphological and behavioral traits, especially body size, nesting biology, diet breadth, and sociality. Phenological traits were infrequently measured and physiological traits were nearly absent from our dataset. Studies investigating climate change effects were also rare. Terminology for trait classifiers were rarely defined, presenting obstacles to data aggregation. We present a roadmap toward open sharing and consolidation of bee trait data, highlighting best practices for standardizing data presentation and making datasets accessible. Along with our review, we present an aggregated morphological trait dataset compiled from our focal studies, representing ___ bee species globally and serving as a template for standardized bee trait data presentation. This framework will facilitate data homogenization and lays the groundwork for standardized and open trait data collection and sharing to advance bee ecological research. 

### Contents

* **Supplementary Table 1**
  Summarized information on functional traits commonly measured in bee ecological studies, with their functional significance, common methods of measurement in bee studies, and common states for traits involving categorical data. We additionally highlight traits that have been infrequently measured in functional trait studies (e.g., desiccation resistance, thermal tolerance, coloration), but which merit further attention due to their relevance to bee fitness and ecological interactions.

* **Supplementary Table 2**
  Metadata from 97 studies analyzed in our review, including citations, the traits analyzed, the types of trait measurements, and the data sources.
  
* **Supplementary Table 3**
  Trait classes, definitions, and associated data sources, where available, for the three most commonly studied behavioral traits: nesting biology, sociality, and diet breadth.

* **Supplementary Table 4**
  Primary morphological data compiled from our focal studies homogenized in a standardized format, described below (see "Guide to the Morphological Dataset and the Data Upload Template).

* **Supplementary Table 5**
  Template for standardized presentation of trait data. Column headers described below (see "Guide to the Morphological Dataset and the Data Upload Template).


### Guide to the Morphological Dataset and the Data Upload Template

Below are definitions of the columns used in the trait dataset template. Where they correspond with the Darwin Core Standard (https://dwc.tdwg.org) they are mapped to those classes. 
  * **basisOfRecord**: [DWC:BasisOfRecord](http://rs.tdwg.org/dwc/terms/basisOfRecord) The specific nature of the data record (character). Eligible values include: ```own measurement/observation```, ```literature record```, or ```ocurrence record```.
  * **catalogNumber**: [DWC:catalogNumber](http://rs.tdwg.org/dwc/terms/catalogNumber) The catalog number of the specimen (character and numeric), if applicable.
  * **recordNumber**: [DWC:recordNumber](http://rs.tdwg.org/dwc/terms/recordNumber) An identifier given to the occurrence (usually, an individual bee) at the time it was recorded. Often serves as a link between field notes and an occurrence record, such as a specimen collector's number, or an individual identifier assigned to a bee during an experiment. This identifier can link individual bees across trait datasets, when multiple functional traits are recorded for a single individual.
  * **recordLevel**: The biological level to which the trait data refers (character). Eligible values include: ```individual```, ```species```, ```population```, or ```colony```.
  * **acceptedNameUsage**: [DWC:acceptedNameUsage](http://rs.tdwg.org/dwc/terms/acceptedNameUsage) The full name, with authorship and date information if known, of the currently valid taxon (character).
  * **acceptedNameUsageID**: [DWC:acceptedNameUsageID](http://rs.tdwg.org/dwc/terms/acceptedNameUsageID) An identifier for the name usage (documented meaning of the name according to a source) of the currently valid taxon (character.
  * **traitName**: The relevant functional trait (character). Eligible values include: ```sociality```, ```nesting location```, ```diet breadth```, ```body size```, ```thermal tolerance```,```desiccation resistance```,```phenology```,```tongue length```,or ```pilosity```.
  * **traitDataType**: The class of functional trait data recorded (character). Eligible values include: ```integer```, ```real number```, or ```character```.
  * **traitDataType**: The unit of measurement of the data (character). Examples include: ```mm```,```deg C```,```hours```, or ```NA``` for character data.
  * **value** The value of the trait measurement (real number, integer, or character). Examples include: ```14```,```22.534```, ```eusocial``` or ```below ground```
  * **valueMeasure**: The type of value represented in the "value" column (character). Eligible values include: ```single observation```, ```mean```,```median```,```min```, ```max```,or ```description```.
  * **variance**: A measure in the variance of the value measurement, if applicable, typically for reported mean values (real number). 
  * **varianceMeasure**: The type of value represented in the "variance" column, if applicable (character).  Examples include: ```std dev```, or ```std error```.
  * **sampleSize**: The relevant sample size used for the value measure, if applicable (integer). Typically applies for reported mean values.
  * **treatment**: The experimental treatment group relevant to the value measure, if applicable (character).
  * **methodName**: The name of the method used to measure the trait (character). Examples include: ```CTmax```, ```mark-recapture```, or ```ITS measurement```.
  * **methodDescription**: A short description of the methods used (character). For example: "Intertegular measurements taken from images using ImageJ".
  * **note**: Any relevant information not included in the above categories, if applicable (character).
  * **study**: A unique name referring to the study in which the data were collected, likely uniting multiple lines of entered data (character). This entry is particularly useful for uniting datasets not yet published. For example: "Ostwald Thermal Tolerance 2022".
  * **reference**: A formatted citation for the reference including the relevant data, if applicable (character). APA citation format preferred. For example: "Hamblin, A. L., Youngsteadt, E., Lopez-Uribe, M. M., & Frank, S. D. (2017). Physiological thermal limits predict differential responses of bees to urban heat-island effects. Biology Letters, 13, 0125."
  * **referenceDOI**: The digital object identifier (DOI) of the above reference, if applicable (character).
  * **locality**: [DWC:locality](http://rs.tdwg.org/dwc/terms/locality) The specific description of the place (character). Examples include: ```Bariloche```,```25 km NNE via Ruta Nacional 40 (=Ruta 237)```, ```Olympic National Park```.
  * **decimalLatitude**: [DWC:decimalLatitude](http://rs.tdwg.org/dwc/terms/decimalLatitude) The geographic latitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of a location (real number).
  * **decimalLongitude**: [DWC:decimalLongitude](http://rs.tdwg.org/dwc/terms/coordinateUncertaintyInMeters) The geographic longitude (in decimal degrees, using the spatial reference system given in geodeticDatum) of the geographic center of a location (real number).
  * **coordinateUncertaintyInMeters**: [DWC:coordinateUncertaintyInMeters](http://rs.tdwg.org/dwc/terms/decimalLongitude) The horizontal distance (in meters) from the given decimalLatitude and decimalLongitude describing the smallest circle containing the whole of the location (real number). Leave the value empty if the uncertainty is unknown, cannot be estimated, or is not applicable (because there are no coordinates). Zero is not a valid value for this term.
  * **country**: [DWC:country](http://rs.tdwg.org/dwc/terms/country) The name of the country or major administrative unit in which the location occurs (character).
  * **stateProvince**: [DWC:stateProvince](http://rs.tdwg.org/dwc/terms/stateProvince) The name of the next smaller administrative region than country (state, province, canton, department, region, etc.) in which the location occurs (character).
  * **county**: [DWC:county](http://rs.tdwg.org/dwc/terms/county) The full, unabbreviated name of the next smaller administrative region than stateProvince (county, shire, department, etc.) in which the location occurs (character).
  * **eventDate**: [DWC:eventDate](http://rs.tdwg.org/dwc/terms/eventDate) The date-time or interval during which an Event occurred. For occurrences, this is the date-time when the event was recorded (character, real number, or integer). For measurements, this is the date-time when the measurement was taken. Examples include: ```1963-03-08T14:07-0600``` (8 Mar 1963 at 2:07pm in the time zone six hours earlier than UTC),```2018-08-29T15:19``` (3:19pm local time on 29 August 2018), ```1906-06``` (some time in June 1906).
  * **sex**: [DWC:sex](http://rs.tdwg.org/dwc/terms/sex) The sex of the biological individual(s) represented in the Occurrence (character). Examples include: ```male```,```female```,```hermaphrodite```.
  * **lifeStage**: [DWC:lifeStage](http://rs.tdwg.org/dwc/terms/lifeStage) The age class or life stage of the bee at the time the occurence or measurement was recorded (character). Examples include: ```adult```,```egg```,```larva```,```pupa```.
  * **associatedTaxa**: [DWC:associatedTaxa](http://rs.tdwg.org/dwc/terms/associatedTaxa) A list (concatenated and separated) of identifiers or names of taxa and the associations of this occurrence to each of them (character). This is particularly relevant for occurences related to diet breadth. Examples include: ```host:Helianthus annuus```,```host:gbif.org/species/2888380```.

## Citation
  
## Acknowledgements
The following organizations made this work possible:
[NSF](https://nsf.gov) for their support and funding of [Big-Bee](https://www.idigbio.org/wiki/index.php?title=TCN:_Extending_Anthophila_research_through_image_and_trait_digitization_(Big-Bee)&mobileaction=toggle_view_desktop), Extending Anthophila research through image and trait digitilization. ([NSF:DBI:2102006](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2102006&HistoricalAwards=false))

<a href="https://www.idigbio.org/wiki/index.php?title=TCN:_Extending_Anthophila_research_through_image_and_trait_digitization_(Big-Bee)&mobileaction=toggle_view_desktop"><img src="https://www.idigbio.org/wiki/images/8/84/Big-Bee-logo-2022.png" class="inline-image" style="height: 6em;"></a>
<a href="https://nsf.gov"><img src="https://big-bee.ccber.ucsb.edu/images/NSF_4-Color_bitmap_Logo-small.png" class="inline-image" style="height: 6em;"></a> 
