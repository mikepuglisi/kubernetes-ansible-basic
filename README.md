# Kubernetes-Cluster-Ansible

This repository contains different ansible-playbooks that can be used to setup a Kubernetes Cluster with Ubuntu 18.04 nodes.

A detailed description is available in my blog: https://www.dev-eth0.de/blog/2018/04/01/kubernetes-cluster-ansible.html

## tl;dr
Configure your inventory and run the following commands:

* `ansible-playbook -i inventory kube-disable-swap.yml`
* `ansible-playbook -i inventory kube-install-software.yml`
* `ansible-playbook -i inventory kube-setup-cluster.yml`
* `ansible-playbook -i inventory kube-self-hosted-recovery.yml`


Afterwards you can use the `kubectl` command using the kubemaster node's `root` account.


## Attributions
The ansible files are based on the work of `bsder` published on digitalocean.com:
https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-1-11-cluster-using-kubeadm-on-ubuntu-18-04
