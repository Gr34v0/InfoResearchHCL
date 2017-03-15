# Research Topics
This is a quick Repo designed to hold just the ReadMe.md which contains some information I was requested to research on DevOps, the Netlist File format, the REST API and the simlarities and differences between MongoDB and CouchDB.

1. DevOps is a compound "word" originating from the terms "Software **Dev**elopment" and "Information Technology **Op**eration**s**" and is meant to reflect the communication and teamwork between software developers and IT professionals, while optimizing and automating the delivery and infastructure changes of software delivery. The concept of DevOps is a cultural and environmental way of thinking that is similar to forms of Agile Development but focuses more on organization due to the larger amounts of software building and release that come from Agile concepts. Benefits of implementing a DevOps structure in a company have been (but not limited to) a shorter time to market for a product, better product quality, rapid experimentation and development, and increased customer satisfaction. Three cultural changes must take place in order to adopt DevOps into a company culture, according to Gene Kim in his "Three Ways Principles" concept. The first change must be in systems thinking; The change emphasis is on the performance of the entire system, as opposed to individual departments. The second change must be in amplifying feedback loops; Listening to, learning from, and increasing feedback from the teams involved in the company to increase communication amongst the teams and the customers involved. The third change must be in company culture, and keeping the experimentation and subsequent learning experience; The changes in risk taking attiute, communication and practice have to be a constant part of the way the company thinks.

* Loukides, Mike (2012-06-07). "What is DevOps?"
* Chen Lianping (2015). "Coninutous Delivery: Huge Benefits, but Challenges Too" IEEE Software 32
* Kim, Gene. "The Three Ways: The Principles Underpinning DevOps"

2. Netlist Files are simple files that are meant to represent a circuit design to be used on a PCB. They consist of a list of terminals (pins) of the components in a circuit and a list of the conductors that connect the terminals. When two or more terminals are connected by a conductor, that conductor is called a net. There are a few versions of netlists which can be physical or logical, instance based or net based, flat or heirarchical, and if the netlist is heirarchical it can be folded or unfolded. A folded hierarchy lets one definition represent several instances, whereas an unfolted hierarchy has one-to-one definition to instance representation.

* https://en.wikipedia.org/wiki/Netlist
  
3. A REST API stands for a "**Re**presentational **S**tate **T**ransfer" API. REST is resource based which means that within the API, things and nouns are referenced rather than actions and verbs (person, user, address resources rather than methods and actions). Reprentations are how resources are manipulated. Clients can hold representations of resources as JSON, XML, CSV and other types of information formats, and can then modify resources on a server, given permission. The Uniform Interface defines the communication between the client and server via a communication method such as HTTP which has verbs such as GET, PUT, POST and DELETE and the URIs (Uniform Resource Identifiers) that are the resource names that are being dealt with. A requirement of REST is that it is stateless. The server contains no state data, and each request has enough context information to process a message properly. This is called having a "Self-descriptive message". The only state of the system is held on the client. A client will not always have direct connections to a server, but the Uniform Interface is the link between the two. This means that when writing a RESTful application, you need to assume that the information being sent to the client is not always from the server, and could be cached or modified by external software or hardware. All the client knows is the Uniform Interface and the information that's being recieved from said interface. Code On Demand can allow a server to send code logic such as Java or Javascript to the client for the client to execute on behalf of the server. In order for an application to be truely RESTful, it must comply with the following constraints; The application must be Scablable, Simplistic, Modifiable, Visible, Portable and Reliable. 

* Fredrich, Todd (2012-05-30). "Intro to REST (aka. What is REST Anyway?)"

4. MongoDB and CouchDB are similar database frameworks that use the NO-SQL model, meaning the data stored in the database is Document-Oriented. The following is a table of the differences between MongoDB and CouchDB.

|            | CouchDB      | MongoDB  |
|:---------- |:------------:|:--------:|
| Data Model     | Document-Oriented JSON  | Document-Oriented BSON |
| Interface      | HTTP/REST      | Custom TCP/IP protocol   |
| Object Storage | Database contains Documents | Database contains Collections that contain Documents |
| Query Method   | Map/Reduce (JS + others) creating Views + Range queries | Map/Reduce (JS) creating collections Object-Based query language |
| Replication    | Master-Master with custom conflict resolution functions | Master-Slave |
| Concurrency    | MultiVersion Concurrency Control | Update in-place |
| Language       | Erlang | C++ |



