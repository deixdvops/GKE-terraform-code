# GKE-terraform-code
## This code is used to create a GKE cluster.
## After the cluster is created, you can use this command: 
## $gcloud container clusters get-credentials $(terraform output -raw kubernetes_cluster_name) --region $(terraform output -raw region)  
## to retrieve the access credentials for your cluster and automatically configure kubectl.
