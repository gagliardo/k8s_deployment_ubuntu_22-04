# k8s_deployment_ubuntu_22-04
Bash script to install a kubernetes cluster on Ubuntu Server 22.04


This bash script will install a Kubernetes Vanlilla cluster on your Ubuntu Server 22.04

## Requirements
- at least 2 Ubuntu Server 22.04 instances
- a coffee (Italian espresso is enough, because you need less than 1 minute to get it up and running :)

## Run the script

### Master node

```
sudo -i
bash <(curl -s https://raw.githubusercontent.com/gagliardo/k8s_deployment_ubuntu_22-04/main/install_master_ubuntu-22-04.sh)
```

### Worker node(s)

```
sudo -i
bash <(curl -s https://raw.githubusercontent.com/gagliardo/k8s_deployment_ubuntu_22-04/main/install_worker_ubuntu-22-04.sh)
```

## Notes

- This script install a vanilla k8s cluster using Kubeadm with containerd as runtime and flunnel as CNI
- Based on the cluster installation script from killer-sh CKS course
