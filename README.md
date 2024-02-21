# SoftwareAG-API-Gateway-Knowledge

## SoftwareAG-API-Gateway Knowledge Dump
## Deployed as Container
- [x] Docker Desktop
  - Docker Desktop will be using local laptop resources CPU & RAM. Advice to proceed with care if Resources are demanding.
  - Application will be compiled into Images and be deployed as an container to work as a running Application.
  - Storages will be stored in Volume.
  - Everytime container was deleted, Data imprinted during container runtime will not be persisted/remained
  - Storage is used to persist Datas created after container runtime.
### Basic Knowledge to know.
  + docker commands
  + wsl if using windows
  + docker desktop
  + dockerfile build knowledge
  + airgapped environment understanding
- [x] OpenShift Container Platform (OCP)/ Code Ready Container (CRC) / Origin Kubernetes Distribution (OKD) / Kubernetes (k8s)
  - is a virtual cloud platform system created using virtual machines with server resources. Production usage is highly recommeded to deploy into this platform due to the capability settings which includes high availablilty and lightweight deployments.
  _
- [x] k3d

# Why API Gateway is implemented?
+ It acts as a middleware for communication between frontend to backend devices.
+ Backend Device will never be expose to frontend interactively with the help of API Gateway.
+ Authentication/Authorization rights can be applied to API Gateway allowing backend to be secured on top of their own security measures.
+ Management on APIs being used can be made easy if there is proper managing system.

# Software/Application used
## 1. Integration Server
### Description for Integration Server
+ Integration Server roles in API Gateway application is simple, it acts as a middleware where all the API Gateway API created in API GatewayManagement Portal are being hosted. 
+ The API Gateway Hostname that is being requested by RESTAPI Consumer/Caller/Requesters.
+ Consumer Hostname will not be exposed to Consumer/Caller/Requester.
+ IS Services can be created using Designer Software
## 2. API Gateway Management Portal
### Description for API Gateway Management Portal
+ API Gateway which will "Duplicate" Backend Hostname
+ Allow mTLS/TLS connection acting as 1st layer of security
+ API Gateway Key acting as a 2nd layer of security
+ And many other policy/security measures can be applied to make Backend Access restricted and safe.
+ LDAP and SSO such as KeyCloak can be linked to API Gateway as a User Management.
## 3. ElasticSearch
### Description for ElasticSearch
+ ElasticSearch is a document oriented database.
+ Mainly based on Indexing of data.
## 4. Kibana
### Description for Kibana
+ Act as a Dashboard as well as management of ElasticSearch Cluster.
+ Kibana has a User Interface to view analytics and edit elasticsearch cluster settings.


## Image Location
## Full Pack with All Neccessary Software
```
docker pull softwareag/apigateway-trial
```
## Minimal Version of ApiGateway
```
docker pull softwareag/apigateway-lean-trial
```
```
docker login registry.connect.redhat.com
Username: {REGISTRY-SERVICE-ACCOUNT-USERNAME}
Password: {REGISTRY-SERVICE-ACCOUNT-PASSWORD}
Login Succeeded!

docker pull registry.connect.redhat.com/elastic/elasticsearch:8.12.1-9ac0f4a5
```
```
docker login registry.connect.redhat.com
Username: {REGISTRY-SERVICE-ACCOUNT-USERNAME}
Password: {REGISTRY-SERVICE-ACCOUNT-PASSWORD}
Login Succeeded!

docker pull registry.connect.redhat.com/elastic/kibana:8.12.1-9ac0f4a5
```
# Standard Step by Step Requirements/Thoughts on Tasks
- [ ] Deploy
- [ ] Define Requirement
- [ ] Set Security Measures requirements.
- [ ] Execute Security Measures.
- [ ] Execute Requirement required.
- [ ] Test case involving Security Measures
- [ ] Test Case involving Requirement Required.
