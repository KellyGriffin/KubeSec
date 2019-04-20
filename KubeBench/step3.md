Let’s view the cluster details. We’ll do that by running *kubectl cluster-info*:

`kubectl cluster-info`{{execute}}

We have a running master.
To view the nodes in the cluster, run the *kubectl get nodes* command:

`kubectl get nodes`{{execute}}

We will now download and install the AquaSec OpenSource project called Kube-Bench.  This will run on the Cluster and allow us to run Master and Node based scanning to look for any Kubernetes security risks. 

``docker run --rm -v `pwd`:/host aquasec/kube-bench:latest install``{{execute}}

`./kube-bench master`{{execute}}

`./kube-bench node`{{execute}}