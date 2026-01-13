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

## Project Artifacts & Documentation
This repository includes multiple forms of documentation to present the project clearly at different levels of detail:

### 1. Gamma Presentation (Visual Overview)
A concise, visual walkthrough of the project created using Gamma AI.
- Summarizes the API testing approach, coverage, and business value
- Intended for quick understanding by recruiters and hiring managers

📄 File: `API-Automation-Project-Contact-List-API.pdf`

### 2. Detailed PDF Documentation
A comprehensive, step-by-step document covering:
- API endpoints and test scenarios
- Authentication flow using JWT
- Environment variable handling
- Positive and negative test cases
- Assertions and validations strategy

📄 File: `Postman-API Testing-2.pdf`

### 3. Postman Collections & Environment Files
Runnable Postman artifacts included for hands-on validation:
- Postman collection JSON
- Postman environment JSON
- Can be directly imported into Postman or executed via Newman

