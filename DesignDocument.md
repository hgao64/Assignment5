# Design Document


**Author**: \<team69\>

## 1 Design Considerations

### 1.1 Assumptions

* The Payment and Reward Management System (PReMS) is designed to run on android operating system.
* The stall manager is the only user of PReMS.
* All transactions made by the customers are done through credit card.
* All transactions by a specific customer are made using a single credit card.
* The credit card is scanned with the help of a credit card scanner which is attached to the computer system.
* Credit card transactions are processed through a third party payment processing service provider.
* Internet service will be used to establish connectivity between stall manager and customers (manager will send notification emails to the customers). 


### 1.2 Constraints

* Since PReMS allows transactions using only credit card, cash cannot be accepted for any purchase.
* Customers can use only one credit card for all their transactions.
* At this point, PReMS is designed to be used by a single user. Multiple users cannot use PReMS.
* PReMS can only be installed on the systems supporting android OS.
* If the internet connection breaks, system is unable to make the connectivity between stall manager and customers.

### 1.3 System Environment

* System on which PReMS application will be running must support android operating system.
* Credit card scanner must be attached to the computer system.
* System's hardware must be capable to connect with a payment-processing service provider that can process credit card transactions.
* Internet connection must be available for the system to send emails to the customers.

## 2 Architectural Design

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

## 3 Low-Level Design

### 3.1 Class Diagram

<img src="ClassDiagram.jpeg" width="640" height="480"/>



### 3.2 Other Diagrams


## 4 User Interface Design
 <img src="UIdiagram1.jpeg" width="640" height="830"/>

<img src="UIdiagram2.jpeg" width="640" height="830"/>




