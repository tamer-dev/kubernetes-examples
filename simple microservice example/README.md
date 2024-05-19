## Example Voting App on Kubernetes
This just example to run multi tier app (microservices app)

This is based on the original [example-voting-app](https://github.com/dockersamples/example-voting-app) repository from the [docker-examples](https://github.com/dockersamples) GitHub page

and modified it to work on the Kubernetes cluster.

to run this app (by pod configurations )

`cubectl create -f voting-app-pod.yaml `

`cubectl create -f voting-app-service.yaml`

`kubectl create -f redis-pod.yaml`

`kubectl create -f redis-service.yaml`

`kubectl create -f worker-pod.yaml`

`kubectl create -f  result-app-pod.yaml`

`kubectl create -f  result-app-service.yaml`

or run this app (by Deployment configurations )


`cubectl create -f voting-app-deploy.yaml `

`cubectl create -f voting-app-service.yaml`

`kubectl create -f redis-deploy.yaml`

`kubectl create -f redis-service.yaml`

`kubectl create -f worker-deploy.yaml`

`kubectl create -f  result-app-deploy.yaml`

`kubectl create -f  result-app-service.yaml`



