---
layout: default
---

## variant to phenotypic feature association


None

URI: [http://bioentity.io/vocab/VariantToPhenotypicFeatureAssociation](http://bioentity.io/vocab/VariantToPhenotypicFeatureAssociation)


![img](http://yuml.me/diagram/nofunky/class/[association|association type;subject;negated;relation;object;qualifiers;publications;provided by]^-[variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-association type >[ontology class|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-subject >[sequence variant|has gene], [genomic entity|has biological sequence]^-[sequence variant|has gene], [sequence variant|has gene]-has gene >[gene|], [gene or gene product|]^-[gene|], [gene|]-in taxon >[organism taxon|], [ontology class|]^-[organism taxon|], [sequence variant|has gene]-in taxon >[organism taxon|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-relation >[relationship type|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-object >[phenotypic feature|], [disease or phenotypic feature|in taxon]^-[phenotypic feature|], [phenotypic feature|]-in taxon >[organism taxon|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-qualifiers >[ontology class|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-publications >[publication|], [information content entity|]^-[publication|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-provided by >[provider|], [administrative entity|]^-[provider|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-frequency qualifier >[frequency value|], [attribute|]^-[frequency value|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-severity qualifier >[severity value|], [attribute|]^-[severity value|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-onset qualifier >[onset|], [attribute|]^-[onset|], [variant to phenotypic feature association|association type;subject;negated;relation;object;qualifiers;publications;provided by;id;name;category;frequency qualifier;severity qualifier;onset qualifier;sex qualifier]-sex qualifier >[biological sex|], [attribute|]^-[biological sex|])
## Mappings


## Inheritance

 *  is_a: [association](Association.html)
 *  mixin: [variant to thing association](VariantToThingAssociation.html)
 *  mixin: [entity to phenotypic feature association](EntityToPhenotypicFeatureAssociation.html)

## Children



## Fields

 * [association type](association_type.html)
    * _connects an association to the type of association (e.g. gene to phenotype)_
    * __range__: [ontology class](OntologyClass.html)
    * inherited from: [association](Association.html)
 * [subject](subject.html)
    * _a sequence variant in which the allele state is associated in some way with the phenotype state_
    * __range__: [sequence variant](SequenceVariant.html) [required]
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
    * _connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object._
    * __range__: [phenotypic feature](PhenotypicFeature.html) [required]
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
 * [frequency qualifier](frequency_qualifier.html)
    * _a qualifier used in a phenotypic association to state how frequent the phenotype is observed in the subject_
    * __range__: [frequency value](FrequencyValue.html)
    * inherited from: [entity to phenotypic feature association](EntityToPhenotypicFeatureAssociation.html)
 * [severity qualifier](severity_qualifier.html)
    * _a qualifier used in a phenotypic association to state how severe the phenotype is in the subject_
    * __range__: [severity value](SeverityValue.html)
    * inherited from: [entity to phenotypic feature association](EntityToPhenotypicFeatureAssociation.html)
 * [onset qualifier](onset_qualifier.html)
    * _a qualifier used in a phenotypic association to state when the phenotype appears is in the subject_
    * __range__: [onset](Onset.html)
    * inherited from: [entity to phenotypic feature association](EntityToPhenotypicFeatureAssociation.html)
 * [sex qualifier](sex_qualifier.html)
    * _a qualifier used in a phenotypic association to state whether the association is specific to a particular sex._
    * __range__: [biological sex](BiologicalSex.html)
    * inherited from: [entity to phenotypic feature association](EntityToPhenotypicFeatureAssociation.html)
