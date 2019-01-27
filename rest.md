# Understanding REST

> Let's get you started with your first architectural style

## Overview

REST is acronym for REpresentational State Transfer. It is architectural style for distributed hypermedia systems and was first presented by [Roy Fielding](https://en.wikipedia.org/wiki/Roy_Fielding) in 2000 in his famous [dissertation](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm).

We'll introduce you to REST's guiding principles or constraints, _resource_, and a little bit about _HTTP methods_.

<hr>

### So you've heard about REST or RESTful APIs

Now you're confused if those two things are the same or just similar right? Well let me help you out buddy!

The quick answer is — they're supposedly same but people can't just follow rules. Let me elaborate: If you don't know yet,
software architectural styles usually have their own guiding constraints or principles to follow. **REST** has six of them, and if
you are able to follow the said constraints without any breaking changes, your approach will be considered **RESTful**.

But before I list down those constraints, you should read about _resource_ first and how they are the key abstraction of information
in this architectural style.

### Resource and Resource Methods

Keep in mind that any information that can be named can be a _resource_: a document or image, a temporal service, a collection of other resources, a non-virtual object (e.g. a person), and so on. REST uses a resource identifier to identify the particular resource involved in an interaction between components.

The state of resource at any particular timestamp is known as _resource representation_. A representation consists of data, metadata describing the data and hypermedia links which can help the clients in transition to next desired state.

The data format of a representation is known as a _media type_. The media type identifies a specification that defines how a representation is to be processed. A truly RESTful API looks like hypertext. Every addressable unit of information carries an address, either explicitly (e.g., link and id attributes) or implicitly (e.g., derived from the media type definition and representation structure).

