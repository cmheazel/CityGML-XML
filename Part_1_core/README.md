# Standard template

## Content

This folder contains the text for the standard

* standard_document.adoc - the main standard document with references to all sections
* remaining adocs - each section of the standard document is in a separate document: follow directions in each document to populate
* figures - figures go here
* images - Image files for graphics go here. Image files for figures go in the "figures" directory. Only place in here images not used in figures (e.g., as parts of tables, as logos, etc.)
* requirements - directory for requirements and requirement classes to be referenced in clause_7_normative_text.adoc
* code - sample code to accompany the standard, if desired
* abstract_tests - the Abstract Test Suite comprising one test for every requirement, optional
* UML - UML diagrams, if applicable
 
## Conformance Class Mapping

Concepts which are severable in the Conceptual Model may not be severable in an encoding of that model. therefore, there may not be a one-to-one mapping of Conceptual Model Conformance Class to Implementaion Specification Conformance Class. However, a mapping must be supplied. The following table provides the first step in that mapping. It maps Conceptual Model Conformance Classes to the Implementation Specification(s) where that Conformance Class is implemented.

|Conceptual Model  |Encoding Specification |Comments 
| -- | -- | -- |
|ADE |Part 0: Core | 
|Appearance |Part 1: Appearance | 
|Bridge |Part 2: Bridge | 
|Building |Part 3: Building | 
|City Furniture |Part 4: City Furniture |
|City Object Group |Part 0: Core |
|Construction |Parts 2, 3, and 9 |Construction concepts are realized through the child requirement classes.  
|Core |Part 0: Core |  
|Dynamizer |Part 0: Core |  
|Generics |Part 0: Core |  
|Land Use |Part 5: Land Use |
|Point Cloud |Part 6: Point Cloud |
|Relief |Part 7: Relief |
|Transportation |Part 8: Transportation | 
|Tunnel |Part 9: Tunnel |
|Vegetation |Part 10: Vegetation |
|Versioning |Part 0: Core |  
|Water Body |Part 11: Water Body | 




## Building

To produce the HTML of the standard run `asciidoctor --safe -a data-uri -o
standard_document.html standard_document.adoc`.

To produce the PDF of the standard run `asciidoctor-pdf --safe -o
standard_document.pdf standard_document.adoc`
