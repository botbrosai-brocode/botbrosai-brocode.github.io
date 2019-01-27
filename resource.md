# Resource as Abstraction of Information

> Before proceeding to REST, you should know about its selected abstraction, resources

## Overview

The key abstraction of information in REST is a resource. Any information that can be named can be a resource: a document or image, a temporal service, a collection of other resources, a non-virtual object (e.g. a person), and so on. REST uses a resource identifier to identify the particular resource involved in an interaction between components.

<hr>

### More on Resource

The state of resource at any particular timestamp is known as _resource representation_. A representation consists of data, metadata describing the data and hypermedia links which can help the clients in transition to next desired state.

The data format of a representation is known as a _media type_. The media type identifies a specification that defines how a representation is to be processed. A truly RESTful API looks like hypertext. Every addressable unit of information carries an address, either explicitly (e.g., link and id attributes) or implicitly (e.g., derived from the media type definition and representation structure).

Also, the resource representations across system should follow certain guidelines such as naming conventions, link formats or data format (xml or/and json).

All resources should be accessible through a common approach such as HTTP GET and similarly modified using a consistent approach.

> Once a developer becomes familiar with one of your API, he should be able to follow the similar approach for other APIs.

### Resource Methods

Other important thing associated with REST is resource methods to be used to perform the desired transition. A large number of people wrongly relate resource methods to HTTP GET/PUT/POST/DELETE methods.

Roy Fielding has never mentioned any recommendation around which method to be used in which condition. All he emphasizes is that it should be uniform interface. If you decide HTTP POST will be used for updating a resource – rather than most people recommend HTTP PUT – it’s alright and application interface will be RESTful.

Ideally, everything that is needed to change the resource state shall be part of API response for that resource – including methods and in what state they will leave the representation.