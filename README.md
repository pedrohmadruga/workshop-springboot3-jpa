# 📘 Project: Jpa Springboot3
## 📖 Project Overview:
> This project is a RESTFUL API designed to manage orders within an e-commerce website, developed in Java 21 and using the H2 database. It was designed to offer safe endpoints to CRUD operations regarding the users.

## Project Structure
├── course/

│   ├── config/

│   ├── entities/

│   ├── repositories/

│   └── resources/

│   └── services/

The project was created to manage HTTP requests. The config package is responsible for loading the needed information for testing in the H2 database, while the rest are responsible for managing the application itself.

The entities package contains the data related to the parts that compose a purchase, such as User, Order, Product, and so on. 

The repositories package contains the operations necessary for CRUD operations. Every repository class inherits from the JPARepository, making it easy and intuitive to do so.

The resources package is the controller package. Within it the GET, POST, PUT and DELETE operations are defined for each relevant entity.

The services package acts as an in-betweener between the repository and the resource. Within it I can call the JPA methods (such as findById) and throw custom exceptions in case it was not possible to do so.

## ⚙️ Features
* REST controllers to control CRUD operations
* Validation to insert or update an entity
* Integration with JPA/Hibernate and H2 database
* Using a separate class to act as the primary key for the OrderItem entity

## 🚀 Tecnologies
* Language: Java 21
* Framework: Springboot3
* Database: H2
* Other dependencies:
  - JPA/Hibernate
