Example of how to deploy a full application with multiple pods and services. More info on the application on : https://github.com/dockersamples/example-voting-app

This application has 5 different pods:
- postgres-pod
- redis-pod
- result-app-pod
- voting-app-pod
- worker-app-pod

two services with type ClusterIp allowing the internal communication between pods:
- redis-service
- postgres-service

and another two services with type LoadBalancer exposing our two websites external:
- voting-app-service
- result-app-service