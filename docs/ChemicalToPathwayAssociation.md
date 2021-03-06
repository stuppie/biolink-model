---
layout: default
---

## chemical to pathway association


An interaction between a chemical entity and a biological process or pathway

URI: [http://bioentity.io/vocab/ChemicalToPathwayAssociation](http://bioentity.io/vocab/ChemicalToPathwayAssociation)


![img](http://yuml.me/diagram/nofunky/class/[association|association type;subject;negated;relation;object;qualifiers;publications;provided by]^-[chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-association type >[ontology class|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-subject >[chemical substance|], [molecular entity|in taxon]^-[chemical substance|], [chemical substance|]-in taxon >[organism taxon|], [ontology class|]^-[organism taxon|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-relation >[relationship type|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-object >[pathway|], [biological process|]^-[pathway|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-qualifiers >[ontology class|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-publications >[publication|], [information content entity|]^-[publication|], [chemical to pathway association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category]-provided by >[provider|], [administrative entity|]^-[provider|])
## Mappings

 * [SIO:001250](http://semanticscience.org/resource/SIO_001250)

## Inheritance

 *  is_a: [association](Association.html)
 *  mixin: [chemical to thing association](ChemicalToThingAssociation.html)

## Children



## Fields

 * [association type](association_type.html)
    * _connects an association to the type of association (e.g. gene to phenotype)_
    * __range__: [ontology class](OntologyClass.html)
    * inherited from: [association](Association.html)
 * [subject](subject.html)
    * _the chemical substance or entity that is an interactor_
    * __range__: [chemical substance](ChemicalSubstance.html) [required]
    * inherited from: [association](Association.html)
 * [negated](negated.html)
    * _if set to true, then the association is negated i.e. is not true_
    * __range__: xsd:boolean
    * inherited from: [association](Association.html)
 * [relation](relation.html)
    * _the relationship type by which a subject is connected to an object in an association_
    * __range__: [relationship type](RelationshipType.html) [required]
    * inherited from: [association](Association.html)
 * [object](object.html)
    * _the pathway that is affected by the chemical_
    * __range__: [pathway](Pathway.html) [required]
    * inherited from: [association](Association.html)
 * [qualifiers](qualifiers.html)
    * _connects an association to qualifiers that modify or qualify the meaning of that association_
    * __range__: [ontology class](OntologyClass.html)*
    * inherited from: [association](Association.html)
 * [publications](publications.html)
    * _connects an association to publications supporting the association_
    * __range__: [publication](Publication.html)*
    * inherited from: [association](Association.html)
 * [provided by](provided_by.html)
    * _connects an association to the agent (person, organization or group) that provided it_
    * __range__: [provider](Provider.html)
    * inherited from: [association](Association.html)
 * [id](id.html)
    * _A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI_
    * __range__: identifier type [required]
    * inherited from: [named thing](NamedThing.html)
 * [name](name.html)
    * _A human-readable name for a thing_
    * __range__: label type
    * inherited from: [named thing](NamedThing.html)
 * [category](category.html)
    * _Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class. In a neo4j database this MAY correspond to the neo4j label tag_
    * __range__: label type
    * inherited from: [named thing](NamedThing.html)
