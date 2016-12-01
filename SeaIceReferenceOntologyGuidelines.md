# Sea Ice Reference Ontology Annotation

Named entity annotation for the sea ice reference ontologies is a specialized task, the ultimate goal of which is to move towards the ability to automatically generate the OWL language ontologies needed not just to facilitate cross-domain data discovery and use; but also to generate open-linked data as well (where appropriate).  As such, the scope of the task is restricted to only annotating those terms from specific sections of the WMO Nomenclature document from which these ontologies were derived:

* Section 1, 
* Section 2 (but not section 2.7 or 2.8), 
* Section 4.2
* Section 4.3.1
* Section 4.3.2
* Section 4.3.4 (but not 4.3.4.1)
* Section 4.3.5
* Section 4.3.6
* Section 4.3.7 (skip 4.3.7.3 through 4.3.7.8 and 4.3.7.10 - 4.3.7.14)

Entities are the main things annotated, while properties are used to describe or characterize relationships between entities and to specify values in these relationships where relevant.  For example, in a discussion about cars and their colors, both the words “car” and “color” would be general entities and there might be the property hasColor,  In that case, the sentence “My car is blue”, would be annotated as:

    ```[My car] is [blue].```  
    
Where [My car] would have the general_entity “car”; [blue] would have the general_entity “color”; and the   property hasColor for the entity [My car] would be [blue].

It should be noted that you can not annotate a property unless there has been a general entity tagged (i.e., can’t say hasColor blue unless “blue” has been tagged as a color).

## The Sea Ice Ontologies

There are many tools that can be used to display the relationships between terms within a suite of ontologies.  Protege is one such tool and the tool that was used in generating the ontologies in the first place.  When displayed, the top level terms are depicted in the figure below.  The part of the ontologies that we are interested in here are the terms under the Sea Ice concept described below (which will be relabeled “ice” in the next version of the ontologies). In other words the ‘forms of floating ice’, the ‘ice with concentration’, and the ‘ice with development stage’ concepts and their subconcepts. 

