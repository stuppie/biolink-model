---
layout: default
---

## planetary entity


Any entity or process that exists at the level of the whole planet

URI: [http://bioentity.io/vocab/PlanetaryEntity](http://bioentity.io/vocab/PlanetaryEntity)


![img](http://yuml.me/diagram/nofunky/class/[named thing|id;name;category]^-[planetary entity|])
## Mappings


## Inheritance

 *  is_a: [named thing](NamedThing.html)

## Children

 *  child: [environmental process](EnvironmentalProcess.html)
 *  child: [environmental feature](EnvironmentalFeature.html)
 *  child: [geographic location](GeographicLocation.html)
 *  child: [geographic location at time](GeographicLocationAtTime.html)


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
