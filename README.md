# Real-Estate-Property-Management-System
Real Estate Property Management System built with Java and Spring Boot. Users can browse properties, manage bookings (create, edit, delete), save favorites, and leave reviews. All data stored in text files. My contribution: full booking module with availability validation.
# Real Estate Property Management System

A Java-based property management application built with **Spring Boot** and file-based storage. The system allows users to browse properties, manage bookings, leave reviews, and handle transactions. It demonstrates core concepts of object-oriented programming, RESTful APIs (if applicable), and data persistence using text files.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Booking Module (My Contribution)](#booking-module-my-contribution)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Features

- **User Management**: Register, login, and role-based access (customer/admin).
- **Property Listings**: Add, view, update, and delete property details.
- **Booking System** (CRUD): Customers can create, view, edit, and cancel their bookings. Availability checks prevent double-booking.
- **Favorites**: Users can save properties to a favorites list.
- **Reviews & Ratings**: Leave feedback on booked properties.
- **Transactions**: Track payment or rental transactions.
- **File-based Storage**: All data is stored in structured text files (`users.txt`, `properties.txt`, `bookings.txt`, etc.).

---

## Technologies Used

- **Java 17** – Core language
- **Spring Boot** – Application framework (for dependency injection and REST endpoints, if any)
- **Maven** – Build and dependency management
- **File I/O** – Data persistence using text files
- **Git & GitHub** – Version control

---

## Project Structure
real-estate-property-management/
├── src/
│ └── main/
│ ├── java/com/realEstate/
│ │ ├── RealEstateApplication.java # Spring Boot entry point
│ │ ├── controller/ # REST controllers (if any)
│ │ ├── model/ # POJOs (User, Property, Booking, etc.)
│ │ ├── repository/ # File-based data access classes
│ │ └── service/ # Business logic
│ └── resources/
│ └── application.properties # Spring configuration
├── data/ # Text files storage
│ ├── users.txt
│ ├── properties.txt
│ ├── bookings.txt
│ ├── favorites.txt
│ ├── reviews.txt
│ └── transactions.txt
├── .gitignore
├── mvnw / mvnw.cmd / .mvn/ # Maven wrapper
├── pom.xml
└── README.md


---

## Booking Module (My Contribution)

I was responsible for the complete design and implementation of the **Booking Management** subsystem.

- **CRUD Operations**: Users can create, view, update, and delete their bookings. Only authenticated customers have access to their own bookings.
- **Validation Logic**: Implemented checks to ensure property availability for the requested dates, preventing overlapping bookings.
- **File Persistence**: Used Java I/O classes to read/write booking records to `bookings.txt` with proper formatting and error handling.
- **User Context**: Integrated with the login session so that operations are scoped to the logged-in user.
- **Testing**: Manually tested edge cases (booking conflicts, editing non-existent bookings, etc.) to ensure robustness.

This module strengthened my understanding of file-based storage, object-oriented design, and user interaction flows in a console or web-based Java application.

---

