This my for testing and building out automated command and control deployments. Kubernetes cluster. I try to adhere to Infrastructure as Code (IaC) and GitOps practices using tools like Ansible, Terraform, Kubernetes, Flux, and GitHub Actions.


## Kubernetes

The core infrastructure is based on k0 with Cillium as the CNI.  All storage is replicated with Longhorn.


## Core Components:

- Networking: Cilium which provides eBF-based networking
- Cilium LB IPAM:  Provides a loadbalancer for the cluster
- Longhorn: Longhorn for storing our perstent volumes and creating HA for pods.
- Automation CI/CD:  Uses Fluxcd to maintain the infrastructure.  Custom images being deployed are built with Gitea actions

This repositoray is related to my blog series published here:

https://www.th3redc0rner.com/infrastructure/


