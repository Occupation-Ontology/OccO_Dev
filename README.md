# OccO_Dev
Development Repo for OccO Occupation Ontology

### Note: dev site version 1: 2/12//22  
The Occupation Ontology (OccO) is an ontology in the domain of human occupations. OccO standardizes and represented all the occupations defined in the Standard Occupational Classification (SOC) developed by the following US Federal agencies:
- Department of Labor 
- Bureau of Labor Statistics
- The O\*NET Program, the United States' primary source of occupational information. 

OccO reflects the data content of the **O\*Net-SOC 2019** taxonomy, and it is developed by following OBO Foundry principles. 

OccO is co-developed by Sam Smith and Oliver He, at the University of Michigan Medical School, Ann Arbor, MI, USA. 

OccO was initially developed as part of the Role Ontology (RoleO) as seen here in BioPortal: https://bioportal.bioontology.org/ontologies/ROLEO. 

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


