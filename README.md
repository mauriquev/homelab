# README

## Introduction

This repository is for my K8s bare metal homelab cluster. I will document the tools and technologies I use as I build an environment to hone and master my cloud/DevOps skills. I designed this project to be a place where I can grow, while also evolving with me as I dive deeper into the Kubernetes, Cloud, DevOps and Microservices.

I plan on following  ‘The Twelve-Factor App’ principles and GitOps fundamentals.

## Hardware and Kubernetes Distribution

I  wanted something that was power efficient and small, so I opted for the Raspberry Pi 5. I also am using an SSD as I wanted a safer storage option than microSD cards.

### Hardware:

- Raspberry Pi 5
- 256 GB SSD (x2)
- Official Raspberry Pi 5 M.2 HAT (x2)

| Node | Usage | Hardware |
| --- | --- | --- |
| Midas | Control-Plane | Raspberry Pi 5 (8GB) |
| Orpheus | Worker  | Raspberry Pi 5 (8GB) |
| TBA | TBA |  |

I am using K3s as my Kubernetes distribution. It works well with ARM and it's lightweight, making it perfect for Pi 5 with its limited resources.

## GitOps

The two most popular GitOps tools are Argo and Flux. They use Git as a single source of truth. I will be testing both tools and see which one meets my needs the best.

**~~Flux:~~**

- ~~Currently the GitOps tool that I am using to manage and deploy my current cluster's K8s objects. I am following the monorepo structure.~~

**Argo:**

- Now my primary GitOps tool going forward.

## CI/CD
- For my current projects, I am using GitHub Actions as my primary CI/CD tool. the CD is moslty handled by Argo ans CI by Actions

## Monitoring
- For monitoring and metrics I opted for kube-prometheus HA inside my cluster. This provides me with cluster metrics and the ability to create custom dashboards.