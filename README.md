# User–Order Microservices

A simple two-service demo showing service-to-service communication in a microservice setup:

- **User Service** (port `5001`) — manages users.
- **Order Service** (port `5002`) — manages orders and calls the User Service to enrich order responses with user details.

Perfect for learning local microservice wiring, HTTP contracts, and simple error handling.

---

## Features

- Two isolated Flask apps with clear responsibilities
- Cross-service HTTP call (`requests` from Order → User)
- Minimal, readable code
- cURL examples for quick manual testing
- Troubleshooting tips for common local issues (e.g., port already in use)

---

## Project Structure
├── user_service.py
├── order_service.py


```
Serverless-WebApp/
├── user_service.py      # User Service
├── order_service.py     # Order Serivice
```




