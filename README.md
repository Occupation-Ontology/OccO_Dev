# OccO_Dev
Development Repo for Occupation Ontology (OccO)

### Note: dev site version 2: 3/15//22 

## Definition and Editor Note from OWL File

### Definition: 
The Occupation Ontology (OccO) is an ontology in the domain of human occupations. OccO standardizes and represents all the occupations defined in the Standard Occupational Classification (SOC) developed by the following US Federal agencies:

* Department of Labor
* Bureau of Labor Statistics
* The O*NET Program, the United States' primary source of occupational information.

OccO reflects the data content of the O*Net-SOC 2019 taxonomy, and it is developed by following OBO Foundry principles.

OccO is co-developed by Sam Smith and Oliver He, at the University of Michigan Medical School, Ann Arbor, MI, USA.  For background on the development of this ontology, see https://observablehq.com/collection/@smithgit/life-ontologies.

OccO was initially developed as part of the Role Ontology (RoleO) as seen here in BioPortal: https://bioportal.bioontology.org/ontologies/ROLEO.

References:
* Standard Occupational Classification (SOC) System: https://www.bls.gov/soc/
* O*Net Resource Center: https://www.onetcenter.org.
* Github Repository: github.com/occupation-Ontology/OccO

### Editor Note:  
The following changes were made to the SOC terms:

Occupations in OWL are classes, and class names are singular, whereas the SOC uses the plural form, to reflect the individuals involved.  So plural terms were changed to singular and made lower-case, and the "and" conjunction was changed to "or."  In SOC quite a number of group labels are the same as child labels, so these parent terms were changed to make unique by adding a suffix to indicate the hierarchy level.  This mainly affected Broad Occupation terms, of which 2** were duplacated in Detailed Occupation, so the broad occupation term has the suffix (broad).  Minor Occupations had 13 duplicates with the suffix (minor), and only one occupation, hunting *** appeared three times as Minor, Broad and Detailed.  A comment was added to indicate the hierarchy level, such as "This occupation in SOC is a Major Group."  This permits extracting all terms at a given hierarch level by using the SPARQL query:
 ***** Add example query here **


The format of SOC occupation ID's is MM-NNNN.dd, wheret the MM indicates Major Group.  The dd suffix was added for the 149 O*Net additions of new occupations.  

The O*Net - SOC taxonomy https://www.onetcenter.org/taxonomy.html has the following hierarchy for 1,569 occupations plus the root "occupation":
Major Groups (23)
  Minor Groups (98)
    Broad Occupations (459)
      Detailed Occupations (867)
        O*Net Additions (149)

The OccO annotations include the following Information Artifact Ontology (IAO) properties:
  IAO_0000111  'preferred term' which is the SOC ID unchanged in the format described above.  Note that the OccO ID requires 8 digits to accommodate the two-digit O*Net suffix. 
  IAO_0000118 'alternative term' is the occupation label as in SOC with capitalization and plural terms.

Revision History

Version 1 - March 2022
Conversion of the O*Net-SOC taxonomy into an OWL ontological structure, follwing the OBO Foundry principles.

Possible enhancements in future releases:
Incorporation of Skills, Abilities and Areas of Knowledge:
Plans to include the O*Net-SOC Skills, Abilities and Knowledge properties to each occupation.  The O*Net-SOC scheme for describing occupations is unique among such classifications by having these additional informative properties, each with a metric for its importance to the occupation, and the level of each that is required for the occupation.  

Reconciliation and Integration with ISOC and Wikidata occupations:
Comparison and reconciliation with other occupation schemas, in particuar the international ISCO system and the semantic web (primarily Wikidata and also DBPedia). 

## Project Folders

### Project Overview
Description of this ontology development project, its motivation, contributors and 
decisions made.
### Comparison of ISCO vs O*Net-SOC
The development of OccO was facilitated by using one of the existing "controlled vocabularies" as its starting reference.  These standards are not ontologically derived, and the hope is that a more ontology-oriented classification of occupations can be accomplished from this OccO development.
### Rationale for OccO use of O*Net-SOC
   OLIVER***  From Pam Frugoli at US DOL / BLS / SOC / O*Net:   
   The U.S. does use the ISCO as one input in development of the SOC.  I think the alignment is fairly close at the more aggregate levels of the hierarchy.  My understanding is that ISCO is designed to be able to collect data from all the nations of the world—and as a result isn’t as detailed in certain areas that may be more important in the economies of the so-called developed nations, but that aren’t significant portions of the economy of other so-called developing nations.  However, it has the advantage of worldwide applicability.  Also for certain types of analysis a more aggregated system, such as ISCO might actually be easier to use, as there are 923 O*NET 2019 occupations.  
### Steps for Converting SOC to OccO

### Folder: ONet-SOC Reference Files
Files in this folder are those directly downloaded from the O*Net Resource Center, saved here as a reference from which all derivative files were created.
### Folder: ONet-SOC Edited for OccO Files
The reference files as converted for use in OccO, the conversion steps shown in Steps for Converting SOC to OccO.
### Folder: ONet-SOC_Ontorat
Two types of file for each Ontorat run: the Excel .xlsx data input file and the Ontorat Settings .txt file.

## References:

- Standard Occupational Classification (SOC) System: https://www.bls.gov/soc/ 
- O\*Net Resource Center:  https://www.onetcenter.org 


