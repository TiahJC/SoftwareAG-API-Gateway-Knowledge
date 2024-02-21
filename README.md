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

# Software/Application used
## 1. Integration Server
### Description for Integration Server
## 2. API Gateway Management Portal
### Description for API Gateway Management Portal
## 3. ElasticSearch
### Description for ElasticSearch
## 4. Kibana
### Description for Kibana


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
