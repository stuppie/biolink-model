---
layout: default
---

## RNA product isoform


Represents a protein that is a specific isoform of the canonical or reference RNA

URI: [http://bioentity.io/vocab/RnaProductIsoform](http://bioentity.io/vocab/RnaProductIsoform)


![img](http://yuml.me/diagram/nofunky/class/[RNA product|]^-[RNA product isoform|has biological sequence;id;name;category;in taxon], [RNA product isoform|has biological sequence;id;name;category;in taxon]-in taxon >[organism taxon|], [ontology class|]^-[organism taxon|])
## Mappings


## Inheritance

 *  is_a: [RNA product](RnaProduct.html)
 *  mixin: [gene product isoform](GeneProductIsoform.html)

## Children



## Fields

 * [has biological sequence](has_biological_sequence.html)
    * _connects a genomic feature to its sequence_
    * __range__: biological sequence
    * inherited from: [genomic entity](GenomicEntity.html)
 * [id](id.html)
    * _A unique identifier for a thing. Must be either a CURIE shorthand for a URI or a complete URI_
    * __range__: identifier type
    * inherited from: [named thing](NamedThing.html)
 * [name](name.html)
    * _A human-readable name for a thing_
    * __range__: label type
    * inherited from: [named thing](NamedThing.html)
 * [category](category.html)
    * _Name of the high level ontology class in which this entity is categorized. Corresponds to the label for the biolink entity type class. In a neo4j database this MAY correspond to the neo4j label tag_
    * __range__: label type
    * inherited from: [named thing](NamedThing.html)
 * [in taxon](in_taxon.html)
    * _connects a thing to a class representing a taxon_
    * __range__: [organism taxon](OrganismTaxon.html)
    * inherited from: [thing with taxon](ThingWithTaxon.html)
