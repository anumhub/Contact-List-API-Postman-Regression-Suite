# Contact List API – Postman Regression Suite

## 1. Project Overview
- API regression test suite built for Contact API using Postman
- Covers JWT authentication , CRUD validations and negative testing

## 2. Tech Stack
- Postman
- Newman (CLI)
- Node.js
- JavaScript Assertions
- Environment variables

## 3. Test Coverage
- Login API with JWT token validation
- GET all contacts
- GET contact by ID
- POST create contact
- PUT update contact
- DELETE contact
- missing token
- 404 not found
- missing requires fields
- invalid formats

## 4. Environment & Data Handling
- Bearer token captured from login response
- contactId stored and reused across requests
- Environment variables used for dynamic execution

## 5. How to Run Tests (Newman)
```bash
newman run postman/ContactList.postman_collection.json \
 -e postman/ContactList.postman_environment.json
```

## 6. Business Impact 
- Converts manual API testing into a repeatable regression suite
- Improves consistency of API validations across environments
- Reduces manual regression effort by an estimated 30–40%
- Enables CLI-based execution for future CI/CD integration

