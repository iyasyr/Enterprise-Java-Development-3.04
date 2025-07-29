# Airline Spring Boot Project

This is a simple Spring Boot application for managing customers, flights, and flight bookings using Spring Data JPA and MySQL.

## Prerequisites

* Java 17 or higher
* Maven (or use the included Maven Wrapper)
* MySQL database running on `localhost:3314` (or update `application.properties` accordingly)
* Lombok plugin enabled in your IDE for annotation support

## Setup

1. **Clone the repository**

   ```bash
   git clone <your-repo-url>
   cd airline
   ```

2. **Configure the database**

   * Edit `src/main/resources/application.properties` if needed to match your MySQL credentials or port.
   * Ensure the database `airline` exists or let Hibernate auto-create it.

3. **Build & Run**

   ```bash
   # Using Maven Wrapper
   ./mvnw clean spring-boot:run

   # Or with installed Maven
   mvn clean spring-boot:run
   ```

4. **Access the application**

   * The service starts on `http://localhost:3315`
   * Hibernate will auto-generate the tables:

     * `customers`
     * `flights`
     * `flight_bookings`
