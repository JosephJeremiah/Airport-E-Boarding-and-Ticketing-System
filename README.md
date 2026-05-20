# Airport E-Boarding and Ticketing System Database

## Overview

The Airport E-Boarding and Ticketing System is a relational database project developed using Microsoft SQL Server and T-SQL. The system was designed to automate and manage airport ticketing operations, passenger reservations, electronic boarding processes, baggage management, and employee administration.

The database follows Third Normal Form (3NF) principles to ensure data integrity, minimize redundancy, and improve system efficiency. The project demonstrates practical implementation of relational database concepts including constraints, indexing, stored procedures, computed columns, and relational mappings.

---

## Aim of the Project

The primary aim of this project is to design and implement a secure, efficient, and scalable airport ticketing and e-boarding database management system capable of handling passenger reservations, flight scheduling, ticket generation, baggage processing, and staff operations.

---

## Objectives

The objectives of this project are to:

- Design a fully normalized relational database in 3NF
- Manage passenger information and reservations efficiently
- Automate ticket issuance and e-boarding processes
- Track baggage information and associated fees
- Improve data consistency using constraints and relationships
- Implement stored procedures for efficient querying
- Enhance database performance using indexing techniques
- Demonstrate practical application of SQL Server database concepts

---

## Technologies Used

- Microsoft SQL Server
- T-SQL
- SQL Server Management Studio (SSMS)

---

## Database Features

### Passenger Management
- Passenger registration
- PNR generation
- Meal preference management
- Emergency contact tracking

### Flight Management
- Flight scheduling
- Origin and destination tracking
- Departure and arrival management

### Reservation System
- Reservation confirmation and cancellation
- Flight-passenger relationship management
- Reservation date validation

### Ticketing System
- Ticket generation
- Fare management
- Seat allocation
- Boarding number management

### Baggage Management
- Baggage tracking
- Weight validation
- Automated baggage fee calculation

### Employee Administration
- Staff role management
- Secure password hashing
- Email uniqueness validation

### Database Optimization
- Index creation for faster queries
- Foreign key constraints
- Check constraints
- Computed columns
- Stored procedures

---

## Database Structure

The project contains the following major tables:

- Employees
- Passengers
- Flights
- Reservations
- Tickets
- Baggage
- AdditionalServices

---

## Sample Functionalities

### Stored Procedures
- Search passengers by last name
- Retrieve reservation details
- Generate boarding information

### Constraints
- Unique email validation
- Reservation date checks
- Flight class validation
- Meal preference validation

### Computed Columns
- Automatic baggage fee calculation
- Additional service fee computation

---

## Sample Query Example

```sql
SELECT P.FirstName, P.LastName, F.FlightNumber
FROM Passengers P
JOIN Reservations R ON P.PassengerID = R.PassengerID
JOIN Flights F ON R.FlightID = F.FlightID;
```

---

## Learning Outcomes

This project demonstrates understanding of:

- Relational database design
- Database normalization (3NF)
- SQL Server implementation
- Data integrity enforcement
- Query optimization
- Real-world database modeling
- T-SQL programming

---

## Future Improvements

Possible future enhancements include:

- Web-based frontend integration
- Real-time flight tracking
- Online payment integration
- Role-based authentication system
- Report generation dashboard
- API integration

---

## Author

Captain Joe

---

## License

This project is for educational and academic purposes.
