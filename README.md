# Kubernetes vote-app deployment

## :scroll: Project description

![schema](img/schema.jpg)

### :pushpin: The Voting App consists of the following components: 

- A Frontend Service that serves the web application to users to vote for their favorite pets (cats or dogs). It is Developed using Python Flask.
- A Redis Service that stores the votes.
- A Worker Service that processes the votes and stores them in the Postgres database.
- A Postgres Service that stores the details of the votes such as the pet name and the number of votes.
- A Result Service that displays the results of the votes. It is Written in Node.js.

### :pushpin: Prerequisites

- A Linux Machine with Docker and Kubernetes installed.


### :pushpin: Project structure

- We create a yaml file for each service and deployment:

```
.
├── db-service.yaml
├── db.yaml
├── redis-service.yaml
├── redis.yaml
├── result-service.yaml
├── result.yaml
├── voting-app.yaml
├── voting-service.yaml
└── worker.yaml
```

- we run minikube start

### :pushpin: Usefull commands:

```
kubectl create -f file-name.yaml # create the deployment or service
```
```
kubectl apply -f file-name.yaml # command uset to apply changes made to a yaml file
```

```
kubectl get pods
```
```
kubectl get services
```
```
kubectl get deployments
```
```
kubectl get replicaset
```
```
kubectl describe pod pod-name
```

```
kubectl delete deployment name-of deployment # use the commmand carrefully
```
```
kubectl delete service service-name
```

![dashboard](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/594326a4-13a3-4a91-a7ec-aa89b90ec7d5)
![deployments](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/6d57fbd1-076d-4b4c-91e8-c59a2cca123a)
![pods](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/2276b61b-59f6-4790-aa37-33c56a47bf69)
![replica-sets](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/a3096dad-23dc-4b24-b3c3-0a6f206bae8b)
![screen-app1](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/fc389f90-a950-40ce-97e1-8342842ea5fb)
![screen-app2](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/f40833ab-82c9-4c50-961f-7f9a91e3da91)
![services](https://github.com/PopFlaviuCiprian/salary_calculator/assets/117381350/df4c0a2b-731d-4da9-b64d-0a61d6d672e0)
