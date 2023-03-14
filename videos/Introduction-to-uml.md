# [Introduction to UML](https://app.pluralsight.com/library/courses/uml-introduction/table-of-contents)

## UML Basics
**Types of Modeling**

Two types:

- Structural modeling shows the physical and conceptual parts of the software

Looking for nouns

- Behavioral modeling shows how it works

Looking for verbs and actions, diagrams like Use Case, Sequence, State, and Activity.

**Basic Building Blocks of UML Diagrams:**

- UML diagrams have two main categories: Things and Relationships
    - "Things" include Classes (rectangular box), Use Cases (elliptical box), Components (rectangular box with an icon on the top right), and Nodes (cube box).
    - Messages represent how different objects or classes communicate with each other.

![Untitled](https://user-images.githubusercontent.com/25881847/225076417-c89a2164-6bcc-4b9f-95e8-9ed133ce36c5.png)

- The return message is designated with a dashed line and an open arrowhead pointing back from the callee to the caller, representing the data that is being returned or the control that's being returned.

![Untitled (1)](https://user-images.githubusercontent.com/25881847/225076501-85790656-38ee-47b9-bf30-6088a2610748.png)

- Relationships are key to understanding how one object or class relates to another, and can be simple associations, such as a simple association and a straight line between two entities.
- The most important details of class diagrams are the numbers at the two endpoints, the asterisk indicating 0 to many elements, the generalization of a class, the implementation of an interface or implement some functionality, and the dependency of an object.
- The arrow points back to the definition and the non-arrow side of the line connects to where the implementation is
- A Dependency identifies some relationship where one object is dependent upon the other

![Untitled (2)](https://user-images.githubusercontent.com/25881847/225076597-e614685f-a08e-48f6-aacc-9fd0c204de97.png)

**Common Extensions**

- Creating the notes can help your readers understand better what you mean by a diagram and they can also help when you're reading a diagram. Make sure you take a look at the notes, and understand what the creator of the diagram wanted you to know.

**Key Considerations**

Keep Diagram Clean

- Readable
- Focused
- Precise

Visualize, Specify, and Document are the goals of our UML diagrams.

Keep the Audience in Mind

- The documents can support our support personnel as bugs come to light, they can look at the documents and maybe better understand where to look in the system to identify or to find the bug that has been identified.

# **Structural Diagrams**

## **Class Diagrams**

Vocabulary

- It identifies the **Vocabulary** of our system. Have a common language between all members of the team.

Relationships

- It defines **Relationships** between entities in our system.

### Class and Interfaces

- Class
    - Represents an Entity
        - Attributes
        - Operations

![Untitled (3)](https://user-images.githubusercontent.com/25881847/225076706-0c148557-2c1d-4d46-8fe8-c954926c0c50.png)

- Interface

![Untitled (4)](https://user-images.githubusercontent.com/25881847/225076738-49ab1f08-312a-4a38-ba32-5b77354ebc87.png)

### **Implementation and Inheritance**

- Implement Interface

We have a Class, Account in this case, that implements that interface.

![Untitled (5)](https://user-images.githubusercontent.com/25881847/225076806-c8bf412f-0f74-4556-84f2-00581bfb3979.png)

- Inheritances (”Is A”)

We're implementing some specifics about an Account class, and we're implementing two specific types of accounts, a Checking Account and a Savings Account.

- Abstract Class
- Concrete Class

![Untitled (6)](https://user-images.githubusercontent.com/25881847/225076885-4fa1e388-6a4c-4954-955e-7bc8f8a520fb.png)

### **Relationships**

- Basic (”Has A”)
    - Multiplicity

![Untitled (7)](https://user-images.githubusercontent.com/25881847/225076937-db38d081-9e1b-426b-95f0-314852df9234.png)

- Aggregation
    - Whole - Part

![Untitled (8)](https://user-images.githubusercontent.com/25881847/225076986-61cc45cc-15f7-48c1-acee-9aeb33f3ec1a.png)

- Composition
    - Ownership

![Untitled (9)](https://user-images.githubusercontent.com/25881847/225077076-1ed99db4-53ef-4370-b5d0-45714eab442b.png)

- Uses

![Untitled (10)](https://user-images.githubusercontent.com/25881847/225077138-3ca11eab-b9c8-4be3-b1df-c9016718cf94.png)

The final diagram:

![Untitled (11)](https://user-images.githubusercontent.com/25881847/225077198-7172be80-51f1-4413-8e9d-54b83db5889d.png)

# **Component Diagrams**

- Component Diagrams help us to understand the structure of our system as far as subsystems or components go.
- It's important that the Developer understands what the Architect and the Business Analyst have in mind as they define these components.

## Basic component

A Basic Component named Online Bill Payer.

- Component

![Untitled (12)](https://user-images.githubusercontent.com/25881847/225077280-aea51db8-d096-4906-b343-3e713c46e06d.png)

- Interfaces

![Untitled (13)](https://user-images.githubusercontent.com/25881847/225077326-52a182da-d377-47cc-bf3e-ea50a5452785.png)

- Three things:
    - Realized: those called ports, this is an interface the Online Bill Payer provides
    
![Untitled (14)](https://user-images.githubusercontent.com/25881847/225077419-ae4fa7bf-42e6-49b3-9b47-704cb234591d.png)
    
    - Required:

![Untitled (15)](https://user-images.githubusercontent.com/25881847/225077488-12384450-0d2b-4562-9a8d-befa18e51595.png)


### Connected Components

- Loosely Connected

Oftentimes this is what we want, this makes our systems more flexible. This is where we can, when we define these loose connections, this is where we can define our pluggable parts of the system. 

- Investment service requires an interface called Payment. It has that half circle, half lollipop, attached to it. And the Online Bill Payer provides or implements or realizes the Payment interface.

![Untitled (16)](https://user-images.githubusercontent.com/25881847/225077536-2fd48b71-fc3f-4c6f-9784-cbf4c2d7ae73.png)

- Tightly Connected

A tight connection between the online bill payer and our instrumentation component

It’s not easy to replace one of these components

Remove one of them requires some rework

![Untitled (17)](https://user-images.githubusercontent.com/25881847/225077600-4386ad41-c3eb-452f-9bd6-2805e4913657.png)

⇒ Create the loose connections where we’ve designed them and create the tight connections  where they are also indicated on the diagram.

## **Package Diagrams**

- This diagram helps to support larger models. As the system grows and our models become larger and larger

### Simple Packages

- Basic

We can see this in other diagrams

![Untitled (18)](https://user-images.githubusercontent.com/25881847/225077670-888b9058-286d-4d31-a87c-0115350f8e00.png)

- Showing (relevant) elements

The AccountServices moves to the top blue box to leave space for relevant elements

It can contain Classe, Interface, Components, Nodes, Diagrams, Packages, Etc.

![Untitled (19)](https://user-images.githubusercontent.com/25881847/225077711-adfeea5a-c07f-4437-8a7f-c87b9cac2194.png)

### Nested Packages

Contained Packages

- In theory, max 2 or 2 deep. But in reality, we can nest them as deep as we want.

![Untitled (20)](https://user-images.githubusercontent.com/25881847/225077773-ece0bd54-773a-4a21-b707-ab5c22c4df19.png)

- Qualified Names: Use double colon - ::

For example, we need to use a fully qualified name to get that RateCalculator

`AccountServes::LoanProcessing::RateCalculator`

## **Deployment Diagrams**

Help us to understand how they map to the physical system and servers in our deployed environment. Identify any special devices that are required for our app to function. And Visualize Hardware and Network Dependencies.

The main users of Deployment Diagrams are often the Product Owners.

### Nodes

1. Processor
- Cubes
    - Nodes in our Deployment Diagrams are represented by boxes or cubes and oftentimes, these have a Processor stereotype attached to them.
    - It's a Processor and it's our database server.
    
![Untitled (21)](https://user-images.githubusercontent.com/25881847/225077865-134df820-2945-4e7a-be2c-5669815fbdaf.png)
    
    - Stereotyped: A server that would be in our datacenter or maybe in the cloud
    - Detailed: We can give it a little bit more detail about a node in our application

![Untitled (22)](https://user-images.githubusercontent.com/25881847/225077920-6fe83a1d-0d9c-4238-98d8-3f9a1a323b2e.png)

2-*: We expect that we will have a minimum of 2 applications, servers and we could have several more, two too many.

1. Devices
- Networks: internet as cloud
- Specialty: scanner, hardwares

![Untitled (23)](https://user-images.githubusercontent.com/25881847/225077980-fcedf97b-4dad-43e6-8265-7b67b9f82548.png)

For example:

- The Deployment Diagram shows a list of the devices that are necessary for the deployment, such as the network, the internet, and the Loan Officer PC.
- It also shows a scanner with a stereotype and links to the Loan Officers PC, as well as a web server, App Server, and Database Server.
- The Loan Officer is likely to be attached to a Branch Server, which is a secure connection between the Branch Server and the App Server. These diagrams help the team understand the physical limits and requirements of the systems.

![Untitled (24)](https://user-images.githubusercontent.com/25881847/225078066-7f00edfe-80dc-407d-a9de-3feaf741c7f6.png)

# **Behavioral Diagrams**

## **Use Case Diagrams**

- Use Case Diagrams are a useful tool for technical architects to identify and model systems, identify important features, and build reusable modules. They can be used to understand better how the Architect may break apart pieces in the system and to create reusable modules that are used across multiple Use Cases.
- The Use Case Diagram is one of the two most commonly used Behavioral Diagrams in the UML. It is used to identify User Tasks, Interactions with people and other systems, and key elements such as operations, functionalities, and user-specific features.

### Actors

**People:** Actors are a special kind of entity that is modeled in a Use Case Diagram. They are often people, such as Sally or Mike or Fred, who are modeled as Roles, something like this:

![Untitled (25)](https://user-images.githubusercontent.com/25881847/225078141-d7b94b15-efeb-453e-8bb4-65d478d4e89b.png)

**Generalization**: It’s also possible to do generalizations about our Actors, here we got a Customer Actor, but we generalized it in two way or inherited from Customer. We got an Individual Customer and a Commercial Customer.

![Untitled (26)](https://user-images.githubusercontent.com/25881847/225078178-713ecc8e-d717-450f-957a-047ade5ecf2e.png)

**Systems:**

Actor interacts with the system to know whether it’s a person or a type of person or roles vs a system.

![Untitled (27)](https://user-images.githubusercontent.com/25881847/225078233-ec2912d5-2a07-4134-924d-b5352ed21bf9.png)

### UseCases

The name of the overall interaction, the overall functionality or outcome that we look for from our system.

For example, we want to pay a bill and we know that there are many steps to doing that

![Untitled (28)](https://user-images.githubusercontent.com/25881847/225078295-1840ce3f-41d2-40bf-874f-12db3d723bb8.png)

- Factor out common processes (<<include>>): it means the Bill Pay Use Case has a dependency on the Authenticate User Use Case.

![Untitled (29)](https://user-images.githubusercontent.com/25881847/225078328-86dc38c4-49ae-400e-9801-ec7dec132550.png)

- Identify optional additions (<<extend>>), it is an extension, The original use case doesn’t know necessarily about the extension, but the extension definitely knows about the base use cases and relies on it and extends the functionality that it provides

### Scenarios

One Use Case may have many scenarios

Things might scenarios for Pay Bill are:

- Steps in process
- Branches
- Extensions
- Exceptions: an exception scenario that says the account that we’ve stipulated to pay our bill from has insufficient funds to pay the bill.

**Use Case vs. Use Case Diagram**

Use Cases are documents that outline the details of pre-Conditions, post-conditions, and the steps taken to implement the Use Case. UMLs are visual representations of how different actors use the Use Cases, and simplified Basic Use Case Diagrams are provided to show the relationship between the Customer and Payment Processing Service. The Customer uses the Pay Bill Use Case, uses the Schedule Recurring Payment Cycle, and uses the Manage Scheduled Payment Use Cases.

The Use Case Diagrams identify the systems in which multiple systems exist. It is important to be aware of the dependency and extended dependency of these systems. There are several ways to manage Scheduled Payment, such as Skip, Terminate, or Modify the Amount.

**Completion of a basic use case diagram**

![Untitled (30)](https://user-images.githubusercontent.com/25881847/225078421-e63c628a-1373-4616-8a16-81ac61f05d2a.png)

## **Sequence Diagrams**

Sequence Diagrams are commonly used to show how objects in a system interact to implement functionality. 

![Untitled (31)](https://user-images.githubusercontent.com/25881847/225078459-40b60ac6-b33b-4fdd-b44b-cbfee696f995.png)

### Classes

- Lifeline

The Lifeline is the amount of time that instance of the class is alive during the operation. It is possible to model objects or specific instances of classes, but for basic diagrams, typically the Classes are used. 

![Untitled (32)](https://user-images.githubusercontent.com/25881847/225078511-a439ca09-6293-4308-a4fa-63558cc42a85.png)

- Focus of Control

Blocks are overlaid on the Lifeline to identify the time the object is being used.

![Untitled (33)](https://user-images.githubusercontent.com/25881847/225078572-ad50d20d-8be4-49e7-994d-7d65d0a07ef4.png)

- Object Lifetime
    - Creation
    - Termination

At Create(), this is where this object is being created.

At Destroy(), this shows how we would model the scenario that we need to create an instance of a class during this operation and that we expect it to be DESTROYED.

![Untitled (34)](https://user-images.githubusercontent.com/25881847/225078626-194a4b83-2c15-4fc9-99a2-e405d3f29f7a.png)

## Messages

A basic message is modeled with a name, message and open/close parentheses, which is going from the Focus of Control line on the Account Service to the Account class. This starts a new focus of Control on the callee. Payee and Asynchronous Message are two types of communication.

![Untitled (35)](https://user-images.githubusercontent.com/25881847/225078690-c56bfa4d-dbfe-4788-a288-6d224917bea6.png)

A synchronous message is when the caller expects the object being called to process the call and return control. The Return line is labeled with left and right arrows. A Self Message occurs when an object calls itself, with the function name being the default name. An asynchronous message is when an object processes a call without blocking the caller.

### Structured Control

**Looping**

This example models a Traffic Light with three states: Red, Yellow, and Green. The Red state turns on the Red light, keeps it on, and then turns on the Yellow light before transitioning to the Green state. The Green state keeps the Green light on until a timer goes off, at which point it transitions to the Yellow state. The Yellow state keeps the Yellow light on until the timer goes off, at which point the Traffic Light transitions back to the Red state.

![Untitled (36)](https://user-images.githubusercontent.com/25881847/225078742-b23a4501-15b3-4a91-b866-57845a8363e3.png)

**Optional**

Lifecycle or objects that need to transition between states based on a triggering event or condition. For example, a user's login session can be modeled as a state machine with states such as "logged out", "logging in", "logged in", and "logging out". They can be used to model complex behaviors and interactions between objects in a system.

![Untitled (37)](https://user-images.githubusercontent.com/25881847/225078788-7a67ebc6-230f-4cf8-af87-56f9cc70b9f0.png)

**Condition**

A Conditional Structure can be used to model scenarios where a decision must be made based on some condition, and the resulting actions will depend on the outcome of that decision. 

![Untitled (38)](https://user-images.githubusercontent.com/25881847/225078874-09f8e289-1cda-4cd2-b03c-6efdbd9e1475.png)

**State Diagrams**

State Diagrams are a useful tool for modeling objects that can transition from one state to another. 

**States**

- Basic

![Untitled (39)](https://user-images.githubusercontent.com/25881847/225078980-0f6ecbd5-a81b-4628-a735-6a11637eb10f.png)

- Internal Behavior
	
![Untitled (40)](https://user-images.githubusercontent.com/25881847/225079050-03e6491a-14e7-437d-a335-53e7cc3f3f59.png)


- Special
    - Initial
    - Final

![Untitled (41)](https://user-images.githubusercontent.com/25881847/225079161-5da66817-a204-4368-adf0-8a2beeec5522.png)

### Transitions

Transitions are usually a simple solid line with an open arrow pointing from one node to another, and can occur due to an operation that has happened on the object. In this case, the operation that caused the state to change is called Reschedule. 

![Untitled (42)](https://user-images.githubusercontent.com/25881847/225079243-65445089-7479-4c51-845a-d5a454a4e8bd.png)

There are two different events that can cause us to transition from one state to another.

### Composite State

- These events may be internal or external to our object, and can lead to a Failed Processing or a Composite State. A Composite State is a special case that has two child states within it, Scheduled and Faulted. It can be modeled by executing a Cancel method.
- This transition can be done by leaving the Idle off of the State Diagram, but it can be messy as any of the states in the Composite State behave the same for this transition.

![Untitled (43)](https://user-images.githubusercontent.com/25881847/225079342-aeacb29b-2438-42d8-a944-64dbd613f648.png)

 Both Cancelled and Completed states then go to Termination or Final states.

# **Activity Diagrams**

![Untitled (44)](https://user-images.githubusercontent.com/25881847/225079416-436659f0-1cea-4ba8-988f-f2bd54479ce5.png)

- Activity Diagrams are similar to flowcharts and are used to model workflows and general operations. They provide details behind a Use Case and help business people understand the flow of the operation.
- The Activity Diagrams are used by the Developer to help build out the parts of the system that are required, the Classes that are needed, and the operations needed to implement them.

## Actions and Activities

An Action is **a single step**, while an Activity, multiple steps, is modeled on an activity Diagram. Actions are broken down into smaller pieces, while activities are Multi Steps. 

- Special
    - Initiation
    - Completion

![Untitled (45)](https://user-images.githubusercontent.com/25881847/225079507-68910013-7f1f-490a-948e-01f553df3b84.png)

### Flow Control

**Decision/ Branch:**

- Flow Control is the process of modeling a flow through a Decision or Branch, which is modeled by a diamond node and represents the statement that is truth for the operation being executed.

![Untitled (46)](https://user-images.githubusercontent.com/25881847/225079572-e36b962b-b2fe-4aac-a403-7d7f3e7fe503.png)

**Fork and Join:**

- Forks and Joins are also used to model parallel behavior, with one flow of operation coming into the diamond and multiple flows going out.

![Untitled (47)](https://user-images.githubusercontent.com/25881847/225079613-0fe2db5a-bc96-4bf2-a75b-753c8960bdcb.png)

