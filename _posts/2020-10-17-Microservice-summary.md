# Data in Microservice

Each service gets its own database (if it needs one)

Services will never, ever reach into another services database

Ok, but why??

### Why database-per-service

- We want each service to run independently of other serices
- Database schema / structure might change unexpectdely
- Some services might function more efficiently with different types of DB's (SQL vs NoSQL)

# Sync communication between services

**Sync**: Services communicate with each other using direct requests

**Async**: Services communicate with each other using events

### Notes on Sync communication

**Pros**

- Conceptually easy to understand
- Service won't need a database

**Cons**

- Introduces a dependency between services
- If any inter-service request fails, the overall request fails
- The entire request is only as fast as the slowest request
- Can easily introduce webs of requests

# Pros and Cons with Asynchronous communication

### Pros

- Service has zero dependencies on other services
- Service will be extremely fast

### Cons

- Data duplication. Paying for extra storage + extra DB
- Harder to understand
