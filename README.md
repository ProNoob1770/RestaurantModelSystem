
# Restaurant Model System

## Table of content 
   - [Frameworks and Language Used](#frameworks-and-language-used)
- [Data Flow](#data-flow)
  - [1. Controller](#1-controller)
  - [2. Services](#2-Services)
- [API Reference](#API-Reference)
- [Data Structures Used ](#Data-Structures-Used)
 - [Key Features](#Key-Features)
   - [1. User CRUD Operations](#1-User-CRUD-Operations)
   - [2. Key Features](#2-Key-Features)
   - [3. Customizable and Extendable](#3-Customizable-and-Extendable)
- [Project Summary](#project-summary)
- [Acknowledgments](#Acknowledgments)
- [Support](#Support)



## Frameworks and Language Used
- Spring Boot
- Java
- Maven

## Data Flow

### 1. Controller
- Controller handles incoming HTTP requests.
- It defines endpoints for adding, retrieving, updating, and deleting user information.


### 2. Services
- The services in the Restaurant Management System are responsible for encapsulating the business logic and operations related to restaurant management. They serve as an intermediary layer between the controllers (which handle HTTP requests) and the repositories (which interact with the database)

### 3.repository
- The repository in the Restaurant Management System project is a crucial component that facilitates the interaction between the application and the database.

## API Reference

#### Post restaurant

```http
  POST resturant
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
|`Request body`  | `restaurant object` | **Required**. list to add. |

#### Get all restaurants

```http
  GET resturants
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| ``      | `` | **Required**. list to  fetch |

#### GET  a restaurant
```http
  Get restaurant/id/{Id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `pathVariable`      | `id` | **Required**. list to  fetch |

#### Update a restaurant

```http
  Put update/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `pathVariable,RequestParam`      | `Integer,String` | **Required**. list to  update. |

#### Delete a restaurant

```http
  Delete delete/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `pathVariable`      | `Integer` | **Required**. list to  remove. |




## Data Structures Used

In the Restaurant Model  System project, the following data structures are used:


- **restaurantId**: A unique identifier for each restaurant. This serves as the primary key in the database table.

- **restaurantName**: Field to store the name of the restaurant.

- **restaurantName**: Field to store the restaurantname of the restaurant. Used for login and identification.

- **restaurantAddress**: Field to store the restaurant's address information.

- **restaurantPhoneNumber**: Field to store the restaurant's phone number.

## Key Features

The User Management System is designed to provide efficient restaurant model. Here are the key features of this application:

### 1. RESTAURANT CRUD OPERATIONS

- **Add restaurant**: Create new restaurant. 

- **Get restaurant by restaurantId**: Retrieve restaurant information by specifying a unique restaurant ID.

- **Get All restaurants**: Retrieve a list of all restaurants in the system.

- **Update restaurant Information**: Modify restaurant information.

- **Delete restaurant**: Permanently remove restaurant  from the system.

### 2. Scalable and Maintainable Architecture

- Utilizes the Spring Boot framework for building robust and scalable applications.

- Follows a well-structured layered architecture, separating concerns between controllers, services, and repositories, ensuring maintainability and testability.



### 3. Customizable and Extendable

- Easily extensible to add more features or attributes to the user profile.


## Project Summary
This project is a Restaurant Model System built using Spring Boot. It provides a set of RESTful API endpoints for managing user information, including adding, retrieving, updating, and deleting user records. The project follows a layered architecture with controllers handling HTTP requests, services containing business logic, and a repository for database operations. User data is stored in a database table with attributes restaurantId, restaurantName, Name, restaurantAddress, and restaurantPhoneNumber.