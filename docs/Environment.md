---
layout: default
---

## environment


A feature of the environment of an organism that influences one or more phenotypic features of that organism, potentially mediated by genes

URI: [http://bioentity.io/vocab/Environment](http://bioentity.io/vocab/Environment)


![img](http://yuml.me/diagram/nofunky/class/[biological entity|]^-[environment|])
## Mappings

 * [SIO:000955](http://semanticscience.org/resource/SIO_000955)

## Inheritance

 *  is_a: [biological entity](BiologicalEntity.html)

## Children

 *  child: [drug exposure](DrugExposure.html)
 *  child: [treatment](Treatment.html)

## Used in

 *  class: [treatment](Treatment.html) references: [drug exposure](DrugExposure.html)
 *  class: [environment to phenotypic feature association](EnvironmentToPhenotypicFeatureAssociation.html) references: [environment](Environment.html)
 *  class: [sequence variant modulates treatment association](SequenceVariantModulatesTreatmentAssociation.html) references: [treatment](Treatment.html)

## Fields

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
