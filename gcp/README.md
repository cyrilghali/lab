# Kubernetes the Hard Way - GCP

1. First you need to install client tools

* Install gcloud. 
* Set a default compute region & zone 
* Install kubectl, cfsslm and cfssljson

2. You need to provide compute resources

* Create a VPC to have a network for your cluster
* Create a subnet so you can assign ip's  to each node to the k8s cluster
* Create firewall rules so you can allows internal communications and external
  ssh icmp and https 
* Create a static ip adress that will be attached to the external LB
* Check firewall rules and ip by listing them (you can filter by name)

*  Create  the kubernetes controllers and workers


3. Provide CA and TLS Certificates:
    * Client and Server Certificates
        * Admin, Kubelet, Controller Manager, Kube Proxy, Scheduler client
          certificate
        * Kubernetes api server certificates
    * Generate a key pair for the Kub Controller Manager to manage service
      accounts

4. Generate kubernetes configuration files for Authentification (KUBECONFIGS)


