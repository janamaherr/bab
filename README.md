# Bab

A food and grocery delivery platform for Cairo: order from verified restaurants or the Bab Mart,
pay by card or cash, and track your driver live. Group orders ("Lamma") let friends order together
and split the bill.

## Tech stack
Java 21 · Spring Boot · PostgreSQL · Flyway · Docker · React + TypeScript (planned)

## Run locally
1. Create a `.env` file in the project root:
   ```
   DB_PASSWORD=your_password
   ```
2. Start the database:
   ```
   docker compose up -d
   ```
3. Start the backend:
   ```
   cd backend
   ./mvnw spring-boot:run
   ```
4. Check: http://localhost:8080/actuator/health returns `{"status":"UP"}`

## Status
Project skeleton in place. Building the MVP: authentication, restaurants, menus, cart and orders.