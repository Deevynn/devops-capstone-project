**As a** developer  
**I need** to set up the development environment  
**So that** I can begin working on the account microservice  

### Details and Assumptions
* The lab environment must have Python, Flask, and required dependencies installed.

### Acceptance Criteria
```gherkin
Given I have access to the online lab
When I set up my development tools and dependencies
Then I should be ready to build and run the microservice

### Read the service
**As a** consumer of the API  
**I need** to retrieve account details by ID  
**So that** I can access a customer's profile information

### Details and Assumptions
* Account must exist in the database  
* Endpoint: GET /customers/<id>  

### Acceptance Criteria
```gherkin
Given a customer ID exists  
When I call the GET endpoint with the ID  
Then I should receive the customer details and a 200 OK status

### Update an account in the service
**As a** user  
**I need** to update account information  
**So that** customer records stay current

### Details and Assumptions
* Endpoint: PUT /customers/<id>  
* Data must be validated  

### Acceptance Criteria
```gherkin
Given a customer exists  
When I send a PUT request with updated information  
Then the customer's data is updated and I receive a 200 OK status

### Delete an account from the service
**As a** system administrator  
**I need** to delete customer accounts  
**So that** I can remove outdated or incorrect records

### Details and Assumptions
* Endpoint: DELETE /customers/<id>  
* Customer must exist  

### Acceptance Criteria
```gherkin
Given a customer ID exists  
When I send a DELETE request  
Then the customer is removed from the database and I receive a 204 status

### List all accounts in the service
**As a** user  
**I need** to view a list of all customer accounts  
**So that** I can see all registered customers

### Details and Assumptions
* Endpoint: GET /customers  
* Should return an array of customer objects  

### Acceptance Criteria
```gherkin
Given there are customers in the database  
When I call the list endpoint  
Then I receive a list of all customer accounts and a 200 OK status

### Containerize your microservice using Docker
**As a** developer  
**I need** to containerize the microservice  
**So that** it can run consistently in any environment

### Details and Assumptions
* Dockerfile should expose the correct port  
* All dependencies must be included  

### Acceptance Criteria
```gherkin
Given I have a working microservice  
When I build and run a Docker container  
Then the service starts and responds to API requests inside the container

### Deploy your Docker image to Kubernetes
**As a** DevOps engineer  
**I need** to deploy the microservice to Kubernetes  
**So that** it can run in a scalable, managed environment

### Details and Assumptions
* Use a Deployment and Service manifest  
* Pull the image from Docker Hub  

### Acceptance Criteria
```gherkin
Given I have a Docker image  
When I apply Kubernetes manifests  
Then the microservice is deployed and accessible via a NodePort or Ingress  





