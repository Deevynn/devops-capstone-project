**As a** customer account manager  
**I need** to add the ability to read, update, delete, and list customer accounts through the REST API  
**So that** other microservices can access and manage customer data effectively  

---

### Details and Assumptions

* The microservice is built using Python and Flask
* The database model and "create customer" endpoint are already implemented
* The online lab environment is being used for development
* API must follow RESTful conventions
* Security and authentication are assumed to be handled separately

---

### Acceptance Criteria

gherkin
Given the account microservice is running in the lab environment  
When a request is made to read, update, delete, or list customer accounts  
Then the correct response should be returned with the appropriate status code and data
