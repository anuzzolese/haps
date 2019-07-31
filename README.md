# HAPS - Holistic Attack Prevention System

The project aims at developing a software solution for automatic “cyber defense” of critical applications.
The system will be able to predict information on possible vulnerabilities thanks to a learning component that will leverage: 

* the source code of the target application (SAST metrics) 
* the information generated during its use ( application log, network status, system status).

The proposed approach, which pushes the state of the art of industrial solutions, aims to drastically improve the effectiveness of the SAST analysis by integrating it with information that is specific to the system under examination and therefore takes into account possible mitigation elements, already in place.

## Description

This repository contains the ontology defined to describe the system in different standardized formats such as RDF, OWL, JSON-LD. There is also a PNG representation of the graph built with Graffoo, a graph modeling tool specific for ontology visualisation, and the related .graphml file to let everyone edit or extend this ontology in yEd.

The .omn format is specific for annotating the entities, which compose the ontology, with software like Protégé.

## Download via content negotiation

You can request the ontology in all the formats mentioned above, including Manchester Syntax, by running this command:

```
curl -L -X GET -H "Accept: <MIME_type>/<MIME_subtype>" https://w3id.org/haps/ont
```

where <MIME_type>/<MIME_subtype> can be:
 * **application/rdf+xml** -> RDF/XML
 * **text/owl-manchester** -> Manchester Syntax
 * **text/turtle** -> Turtle
 * **application/json-ld** -> JSON-LD
 * **text/html** -> HTML

## Built with

* [Graffoo](http://www.essepuntato.it/static/graffoo/specification/current.html) - a graphical notation for OWL ontologies
* [yEd](https://www.yworks.com/yed) - a graph editor
* [Protégé](https://protege.stanford.edu) - an ontology editor and framework for building intellligent systems developed at Stanford

The documentation is available at this URL: http://wit.istc.cnr.it/arco/lode/extract?lang=en&url=https://raw.githubusercontent.com/anuzzolese/haps/master/ont/haps.rdf.

## License
This project is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/).

## Authors

* Andrea Giovanni Nuzzolese
* Alessandro Russo
* Valentina Presutti
* Davide Montanari
