# Design Document


**Author**: \<team69\>

## 1 Design Considerations

### 1.1 Assumptions

* The Payment and Reward Management System (PReMS) is designed to run on android operating system
*The stall manager is the only user using PReMS.
*All the transaction made by the customers are done through credit card.
*All the transaction by one customer are made using single credit card.
*The credit card is scanned with the help of credit card scanner which is attached to the computer system.
*Credit card transaction are processed through a third party payment processing service provider.
*Internet service will be used to establish connectivity between stall manager and customers(send emails to customers). 


### 1.2 Constraints

*Since PReMS allows transaction using only credit card, cash can not be accepted for any purchase.
*Customer can use only one credit card for all his/her purchase/transaction.
*At this point, PReMS is designed to be used by sinle user. Multiple users can not use PReMS.
*PReMS can only be installed on the systems supporting android OS.
*If the internet connection breaks, system is unable to make the connectivity between stall manager and customers.

### 1.3 System Environment

*System on which PReMS application will be running must support android operating system.
*Credit card scanner must be attached to the system which is capable of scanning the credit card.
*System's hardware must be capable to connect with a payment-processing service provider that can process credit card transactions.
*Internet connection must be available for the system to send the emails to the customers.

## 2 Architectural Design

*The architecture provides the high-level design view of a system and provides a basis for more detailed design work. These subsections describe the top-level components of the system you are building and their relationships.*

### 2.1 Component Diagram

<img src="ComponentDiagram.jpg" width="640" height="480"/>

The Component Diagram above is a high level representation of the function components and subsystems required for the PReMS system.  There are two subsystems, the database and android mobile application and three support components to the web application, the Email Managemet, Credit Card Scanner and Payment Processor components.  

####2.1.1 Database Subsystem

The database is comprised of two components or tables which are used to store Customer and Transaction data, hence two components.  The web application calls the database when it needs specific Customer and Transaction data.

####2.1.2 Android Web Application Subsystem

The Android web application comprises of three functional components, the Transaction, Customer and Payment Process components.  These component function cohesively to retrieve and present data to the user of the web application.

####2.1.3 Support Components

There are three support components, the Payment Processor, Credit Card Scanner and Email Management.  The Payment Processor is accepts Customer, Transaction and Credit Card data to charge the credit card of the Customer.  The Credit Card Scanner is a physical component attached to the device to read credit card data.  The Email Management component provides all the necessary functions to compose and send emails to the Customer once a Customer receives an award.

### 2.2 Deployment Diagram

*This section should describe how the different components will be deployed on actual hardware devices. Similar to the previous subsection, this diagram may be unnecessary for simple systems; in these cases, simply state so and concisely state why.*

## 3 Low-Level Design

*Describe the low-level design for each of the system components identified in the previous section. For each component, you should provide details in the following UML diagrams to show its internal structure.*

### 3.1 Class Diagram

*In the case of an OO design, the internal structure of a software component would typically be expressed as a UML class diagram that represents the static class structure for the component and their relationships.*

### 3.2 Other Diagrams

*<u>Optionally</u>, you can decide to describe some dynamic aspects of your system using one or more behavioral diagrams, such as sequence and state diagrams.*

## 4 User Interface Design
 <img src="UIdiagram1.jpeg" width="640" height="480"/>

<img src="UIdiagram2.jpeg" width="640" height="480"/>





