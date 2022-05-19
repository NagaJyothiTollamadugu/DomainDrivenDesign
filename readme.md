  # DOMAIN DRIVEN DESIGN:


 * It is a way way of looking at software from top down.

 * When we are developing a software our focus shouldn't be primaryily on technology, it should be primarily on business or whatever activity we are trying to assist with the software, the domain.

 * Specifically we approach that by trying to develop models of that domain and make our software conformed to that.

* It helps the team create a common model, between the business and IT stakeholders in the company, that the team can use to communicate about the business requirements, data entities, and process models.

 *   The model is modular, extensible and easy to maintain as the design reflects the business model.

  *  It improves the reusability and testability of the business domain objects.


## There are two design tools are there:

# 1)Tactical Design Tools     

* SERVICE ProjectLayers
* Modules

* Design  Paterns

* Oop

* Classes

* Objects

* Exe/Jar/Zip
# 2)Strategic Design Tools
* Domain
* Sub domain
* Service
# Architecture of the Domain Driven Design:

The enterprise application architecture consists of the following four conceptual layers:

   ## User Interface (Presentation Layer): 
                                            Responsible for presenting information to the user and interpreting user commands.

  ## Application Layer:
                         This layer coordinates the application activity. It doesn't contain any business logic. It does not hold the state of business objects, but it can hold the state of an application task's progress.

  ## Domain Layer: 
                   This layer contains information about the business domain. The state of business objects is held here. Persistence of the business objects and possibly their state is delegated to the infrastructure layer.

  ##  Infrastructure Layer: 
                            This layer acts as a supporting library for all the other layers. It provides communication between layers, * implements persistence for business objects, contains supporting libraries for the user interface layer, etc.

                            From a design stand-point, the domain layer should have a well defined boundary to avoid the corruption of the layer from non-core domain layer concerns such as vendor-specific translations, data filtering, transformations, etc. Domain elements should be designed to hold the domain state and behavior correctly. Different domain elements are structured differently based on state and behavior. Table 2 below shows the domain elements and what they contain.
# Design
From a design stand-point, the domain layer should have a well defined boundary to avoid the corruption of the layer from non-core domain layer concerns such as vendor-specific translations, data filtering, transformations, etc. Domain elements should be designed to hold the domain state and behavior correctly. Different domain elements are structured differently based on state and behavior.    

* Entity:
            
  

   “Objects that have a distinct identity that runs through time and different representations. You also hear these called ‘reference objects’.”Although I think the above explanation is quite straightforward, I will give mine.Entities are actors important enough to be unique and have identifiers, simple as that!
* Value Objects:
    
     “Objects that matter only as the combination of their attributes. Two value objects with the same values for all their attributes are considered equal.”That is, it is an object in which we are interested only in its attributes, not its identity. Therefore Value Objects do not have identities and should be objects less complex than entities and immutable, thus facilitating their creation and manipulation.
 
 
 
 * Aggregates:
 
 
    which contain both state (data) and behavior (operations), should have clearly defined state and behavior. At the same time, this behavior should not extend beyond the limits of the object's boundaries. Entities should do most of the work in the use case acting on their local state. But they shouldn't know about too many unrelated concepts.

# Design Patternthat support DDD:

There are several design patterns that help in domain driven design and development. Following is a list of these design patterns:

    * Domain Object (DO)
    * Data Transfer Object (DTO)
    * DTO Assembler
    * Repository
    * Generic DAO's
    * Temporal Patterns


