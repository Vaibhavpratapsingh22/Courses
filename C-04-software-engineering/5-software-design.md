# Chapter 5 - Software Designing
Software design is a mechanism to transform user requirements into some suitable form, which helps the programmer in software coding and implementation. It deals with representing the client's requirement, as described in SRS (Software Requirement Specification) document, into a form, i.e., easily implementable using a programming language.

The software design phase is the first step in SDLC (Software Design Life Cycle), which moves the concentration from the problem domain to the solution domain. In software design, we consider the system to be a set of components or modules with clearly defined behaviors & boundaries.
## Objective of Software Designing
Objectives of Software Design
Following are the purposes of Software design:
<img src="https://static.javatpoint.com/tutorial/software-engineering/images/software-engineering-software-design2.png" height="" width="">
1. **Correctness**: Software design should be correct as per requirement.
2. **Completeness**: The design should have all components like data structures, modules, and external interfaces, etc.
3. **Efficiency**: Resources should be used efficiently by the program.
4. **Flexibility**: Able to modify on changing needs.
5. **Consistency**: There should not be any inconsistency in the design.
6. **Maintainability**: The design should be so simple so that it can be easily maintainable by other designers.
## Object-Oriented Concepts
Object-oriented refers to a programming language, system or software methodology that is built on the concepts of logical objects. It works through the creation, utilization and manipulation of reusable objects to perform a specific task, process or objective.

Objects are the real-world entities that exist around us and the basic concepts such as abstraction, encapsulation, inheritance, and polymorphism all can be represented using UML.
Following are some fundamental concepts of the object-oriented world:
1. **Objects**: Objects represent an entity and the basic building block.
2. **Class**: Class is the copy of an object.
3. **Abstraction**: Abstraction represents the behavior of the real-world entity.
4. **Encapsulation**: Encapsulation is the mechanism of binding the data together and hiding them from the outside world.
5. **Inheritance**: Inheritance is the mechanism of making new classes from existing ones.
6. **Polymorphism**: It defines the mechanism to exists in different forms.
## UML
A picture is worth a thousand words, UML (Unified Modeling Language) is a standard language for specifying, visualizing, constructing, and documenting the artifacts of software systems. UML was created by the Object Management Group (OMG) and UML 1.0 specification draft was proposed to the OMG in January 1997. It was initially started to capture the behavior of complex software and non-software system and now it has become an OMG standard.
 ### Open Source UML Tools
List of some open source UML tools which are available for free:
1. Draw.io
1. AgroUML
2. StarUML
3. BOUML
4. EclipseUML
### Goals of UML
1. Provide users with a ready-to-use, expressive visual modeling language so they can develop and exchange meaningful models.
2. Provide extensibility and specialization mechanisms to extend the core concepts.
3. Be independent of particular programming languages and development processes.
4. Provide a formal basis for understanding the modeling language.
5. Encourage the growth of the OO tools market.
6. Support higher-level development concepts such as collaborations, frameworks, patterns and components.

In conclusion, the goal of UML can be defined as a simple modeling mechanism to model all possible practical systems in today’s complex environment. The above mentioned goals can be completely achieved if your conceptual model is of good quality.

The conceptual model of UML can be completely understood after gaining the complete knowledge of UML building blocks and rules to connect the building blocks. The building blocks of UML can be defined as:

1. Things
2. Relationships
3. Diagrams
### 1. Things
Things are the most important building blocks of UML. Things can be:

1. Structural
2. Behavioral
3. Grouping
4. Annotation

**Structural Things** : Structural things define the static part of the model. They represent the physical and conceptual elements. Below is the brief description of the structural things:
1.  **Class**: Class represents a set of objects having similar responsibilities.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks.png" height="" width="">

3. **Object**: An individual that describes the behavior and the functions of a system. The notation of the object is similar to that of the class; the only difference is that the object name is always underlined and its notation is given below;

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks2.png" height="" width="">

2. **Interface**: Interface defines a set of operations, which specify the responsibility of a class.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks3.png" height="" width="">

3. **Collaboration**: Collaboration defines an interaction between elements.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks4.png" height="" width="">

4.  **Use case**: Use case represents a set of actions performed by a system for a specific goal.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks5.png" height="" width="">

5. **Component**: Component describes the physical part of a system.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks7.png" height="" width="">

6. **Node**: A node can be defined as a physical element that exists at run time.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks8.png" height="" width="">

**Behavioral Things**: A behavioral thing consists of the dynamic parts of UML models. Following are the behavioral things −

1. **Interaction**: A set of operations that describes the functionality of a class, which is implemented whenever an interface is implemented.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks11.png" height="" width="">

2. **State machine**: It defines a sequence of states that an entity goes through in the software development lifecycle. It keeps a record of several distinct states of a system component.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks9.png" height="" width="">

**Grouping Things**: It is a method that together binds the elements of the UML model. In UML, the package is the only thing, which is used for grouping.
1. **Package**: It is the only one grouping thing available for gathering structural and behavioral things.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks12.png" height="" width="">

**Annotation Things**: It can be defined as a mechanism to capture remarks, descriptions, and comments of UML model elements. 
1. **Note**: It is the only one Annotation thing available. A note is used to render comments, constraints, etc. of a UML element.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks13.png" height="" width="">

### 2. Relationship 
 This is another most important building block of UML. It shows how the elements are associated with each other and this association describes the functionality of an application.There are four kinds of relationships available.
1. **Dependency**: It is a relationship between two things in which change in one element also affects the other.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks14.png" height="" width="">

2. **Association**: It is basically a set of links that connects the elements of a UML model. It also describes how many objects are taking part in that relationship.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks15.png" heihgt="" width="">

3. **Generalization**: It can be defined as a relationship which connects a specialized element with a generalized element. It basically describes the inheritance relationship in the world of objects.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks16.png" height="" width="">

4. **Realization**: It can be defined as a relationship in which two elements are connected. One element describes some responsibility, which is not implemented and the other one implements them. This relationship exists in the case of interfaces.

<img src="https://static.javatpoint.com/tutorial/uml/images/uml-building-blocks17.png" height="" width="">

### 3. Diagrams
 All the elements, relationships are used to make a complete UML diagram and the diagram represents a system. The visual effect of the UML diagram is the most important part of the entire process. All the other elements are used to make it complete.

UML includes the following nine diagrams, the details of which are described in the subsequent chapters.

1. Class diagram
1. Object diagram
1. Use case diagram
1. Sequence diagram
1. Collaboration diagram
1. Activity diagram
1. State-chart diagram
1. Deployment diagram
1. Component diagram
## Types of UML Diagrams
Now we will discuss several different types of UML diagrams in detail.
### 1. Class Diagram
Class is a type of static structure diagram that describes the structure of a system by showing the system's classes, their attributes, operations (or methods), and the relationships among objects. A class is represented by a rectangle that contains three compartments stacked vertically—the top compartment contains the class’s name and is mandatory, but the bottom two compartments give details about the class attributes and class operations or behaviors.
The following points should be remembered while drawing a class diagram −
1. The name of the class diagram should be meaningful to describe the aspect of the system.
2. Each element and their relationships should be identified in advance.
3. Responsibility (attributes and methods) of each class should be clearly identified
4. For each class, minimum number of properties should be specified, as unnecessary properties will make the diagram complicated.
5. Use notes whenever required to describe some aspect of the diagram. At the end of the drawing it should be understandable to the developer/coder.

Finally, before making the final version, the diagram should be drawn on plain paper and reworked as many times as possible to make it correct.

 <img src="https://www.researchgate.net/profile/Muhammad_Iqbal_Hossain/publication/255173345/figure/fig1/AS:614317841977382@1523476195594/Class-diagram-of-customer-order-domain.png" height="" width="">

### 2. Component Diagram
Component diagrams are different in terms of nature and behavior. Component diagrams are used to model the physical aspects of a system. Now the question is, what are these physical aspects? Physical aspects are elements such as libraries, files, documents, etc. which reside in a node. Component diagrams are used to visualize the organization and relationships among components in a system. These diagrams are also used to make executable systems.

The following points should be remembered while drawing an component diagram:
1. Use a meaningful name to identify the component for which the diagram is to be drawn.
2. Prepare a mental layout before producing the using tools.
3. Use notes for clarifying important points.

<img src="https://1.bp.blogspot.com/-hZxgZYJKKm8/WtBwUvDQ6gI/AAAAAAAAACg/FzYxeE9alkw7ZecNuvWXB9K4H70H7SXkACK4BGAYYCw/s1600/component-diagram.png" height="" width="">

### 3. Use Case Diagram
Only static behavior is not sufficient to model a system rather dynamic behavior is more important than static behavior. In UML, there are five diagrams available to model the dynamic nature and use case diagram is one of them. Now as we have to discuss that the use case diagram is dynamic in nature, there should be some internal or external factors for making the interaction.

These internal and external agents are known as actors. Use case diagrams consists of actors, use cases and their relationships. The diagram is used to model the system/subsystem of an application. A single use case diagram captures a particular functionality of a system. The following points should be remembered while drawing a use case diagram:
1. The name of a use case is very important. The name should be chosen in such a way so that it can identify the functionalities performed.
2. Give a suitable name for actors.
3. Show relationships and dependencies clearly in the diagram.
4. Do not try to include all types of relationships, as the main purpose of the diagram is to identify the requirements.
5. Use notes whenever required to clarify some important points.

<img src="https://d3n817fwly711g.cloudfront.net/blog/wp-content/uploads/2015/02/A-use-case-template-for-an-ATM-system.png" height="" width="">

### 4. Activity Diagram
Activity diagram is another important diagram in UML to describe the dynamic aspects of the system.
Activity diagram is basically a flowchart to represent the flow from one activity to another activity. The activity can be described as an operation of the system.

The control flow is drawn from one operation to another. This flow can be sequential, branched, or concurrent. Activity diagrams deal with all type of flow control by using different elements such as fork, join, etc. Before drawing an activity diagram, we should identify the following elements:
1. Activities
2. Association
3. Conditions
4. Constraints
<img src="https://media.geeksforgeeks.org/wp-content/uploads/UML-Activity-Diagram-26.png" height="" width="">

### 5. Sequence Diagram
Sequence diagrams describe interactions among classes in terms of an exchange of messages over time. They're also called event diagrams. A sequence diagram is a good way to visualize and validate various runtime scenarios. These can help to predict how a system will behave and to discover responsibilities a class may need to have in the process of modeling a new system.

Start with one of SmartDraw's included sequence diagram templates. You'll notice that all the notations and symbols you need are docked to the left of your drawing area. Simply stamp them to your page and connect the symbols.
<img src="https://i.pinimg.com/originals/d2/53/16/d25316ce459323732e704e5c2ebda3d9.png" height="" width="">

## Summary
 In this chapter we will go through all the main topics in software designing.
Firstly we will study objective of software design, object-oriented concepts. Then we will head towards the main topic i.e Unified Modeling Language(UML) and its different types of diagrams.

In the next chapter we will start with Software Testing.
![Chapter-5](https://img.shields.io/static/v1?label=Finished&message=Software-Design&color=red) ![Chapter-5](https://img.shields.io/static/v1?label=Source&message=www.tutorialpoint.com&color==orange)![Chapter-5](https://img.shields.io/static/v1?label=PRs&message=Welcome&color=blue)
