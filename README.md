# User–Order Microservices

A simple two-service demo showing service-to-service communication in a microservice setup:

- **User Service** (port `5001`) — manages users.
- **Order Service** (port `5002`) — manages orders and calls the User Service to enrich order responses with user details.

Perfect for learning local microservice wiring, HTTP contracts, and simple error handling.

---

## Features

- Two  services with clear responsibilities
- Cross-service HTTP call (`requests` from Order → User)
- Minimal, readable code

---

## Project Structure
```
User-Order-Microservices/
├── user_service.py      # User Service
├── order_service.py     # Order Serivice
```

# API Documentation

## User API


### ➤ Create User
**Curl:**
```bash
curl --location 'http://127.0.0.1:5001/users' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "Tanmay Ranaware",
    "email": "tanmayranware14@gmail.com"
}'
```

**Request Body:**
```json
{
  "name": "Tanmay Ranaware",
  "email": "tanmayranaware14@gmail.com"
}
```
**Response Body:**
```json
{
  "user_id": 5
}




