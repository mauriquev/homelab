# K8s Homelab 

This repository is for my k8s Homelab cluster. I wil be following ‘The Twelve-Factor App’ principles and GitOps fundemantals.

**Goal:** Create a production level cluster that enables me to explore and utilize DevOps tools and technologies while following best practices.
## Distribution 
- k3s lightweight disro on a raspberry pi5.
- Pi5 has limited compute so the distribution meets my needs 


## GitOps

The two most popular GitOps tools are Argo and Flux, they use git as a single source of truth. I will be testing both tools and see which one meets my needs the best. 

**Flux:** Currently the GitOps tool that I am using to manage and deploy my current cluster k8s objects. I am following the monorepo structure.

**Argo:**  Will try it out soon once initial cluster is setup 

## Encrypting Secrets 

As of now I decided to use Sealed Secrets for my secret manifest encryption. Its pretty straight forward and decryption is done my a controller within your own cluster.
## CI/CD

## Monitoring