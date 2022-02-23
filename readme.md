Start Docker for Desktop
In settings -> Kubernetes -> Check "Enable Kubernetes" 
On terminal, use below commands to spinup and tear down, nginx K8s deployment
   kubectl apply -f .\nginx-deployment.yaml   
   kubectl delete deployment nginx-deployment
nginx-deployment contains both deployment as well as service config
deployment config specifies the container to be wrapped inside pod, # of pods, 
service prvoide dns name to the pods, specifies type of service like internal, external, load balancer etc. Even if service is doen pods will exists although one has to manually access through pod IPs