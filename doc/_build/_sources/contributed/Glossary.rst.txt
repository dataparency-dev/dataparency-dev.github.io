Glossary
========

.. _entity:

Entity
------

Any uniquely identifiable collector of data. An abstract concept best understood in the context of its function within the Dataparency server. An entity might be a particular hospital and the documents collected are patient visits. The entity might be a person or some noun. One attribute of an entity is its explicit identity outside the context of Dataparency, e.g. social security number for a U.S. person.  

.. _document:

Document
--------

Any JSON_-compatible text data with a single name value. The value of the single name can be a complex structure, e.g. object or array, or a simple structure, e.g. string. The value can be whatever JSON_ supports. The value can contain other name values in a hierarchy as supported by JSON_. The single name value as a base structure is a constraint on the JSON_ structure by the Dataparency server. 

.. _JSON: https://www.json.org/ 

Relationship
------------

A logical connection between a source entity_ (from) and a target entity_ (to) created via the Dataparency API. It is used by a source entity to attach documents to the target entity. If target entity is a patient and doctor the source, the doctor might be setup in relationship to several patients each of which the doctor would be able to attach documents, e.g. data about visits. 


EDID
----

A Entity Distributed Identifier uniquely identifies an entity_. An EDID can be looked at as a kind of RDID_ where the EDID represents a relationship_ created from the Dataparency server to the entity.


RDID
----

A Relationship Distributed Identifier uniquely identifies a relationship_ between 2 `entities`__

__ entity_


Path
----

A 3 level hierarchy of names organizing a collection of `documents`__ for an entity_ described as
 
	<level 1>/<level 2>/<level 3>. 
	
The path is specified and set when the consumer of Dataparency API attaches a document_ to an entity_. 

__ document_