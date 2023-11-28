# GKE Terraform Code

## Overview

This repository contains Terraform code for creating a Google Kubernetes Engine (GKE) cluster on Google Cloud Platform (GCP). 
After the cluster is created, use the following command to retrieve access credentials and automatically configure `kubectl`:

```bash
gcloud container clusters get-credentials $(terraform output -raw kubernetes_cluster_name) --region $(terraform output -raw region)

