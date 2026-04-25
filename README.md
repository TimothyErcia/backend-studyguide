# Backend Study guide
Repository for all my backend exposures

## Technology
| Language | Framework             | Database   |
|:--------:|:---------------------:|:----------:|
| Node.js  | Express.js            | MongoDB    |
| Golang   | PostgreSQL for Golang | PostgreSQL |
| Python   | FastAPI               | MySQL      |
##

### Goal of the R&D
To familiarize backend stack with the basic CRUD operation, middle end for basic Auth validation, and Cloud Architecture

### Functional Requirements
- Must be able to handle Success response
- Must be able to handle Error response
- Must be able to do validation/authentication
- Must have a cron job/sync service to rotate tokens

### High Level Design
- CRUD operation for v1/route endpoint
- Request and Response when accessing v1/route endpoint
- Authentication validation when accessing v1/route endpoint
- Redis Cache layer
- Rotating token layer/service

### Low Level Design
#### User Model
| id   | name    | password    | api_key        |
|:----:|:-------:|:-----------:|:--------------:|
| UUID | VARCHAR |   SHA256    | rotating token | 

#### Good to have R&D
- GraphQL implementaion
- gRPC implementation
- Multi switching Cloud service
- Design Architecture for Scalability
