# kubernetes-hosted
This project contains learning resources and scripts to create a Kubernetes cluster. The purpose of this project is to learn kubernetes deployment, how to configure a HA cluster, and to deploy the simple containerized app to the kube cluster. The simple containerized app: https://github.com/jdchandler88/containerexperiment

## Learning Resources
* https://serverfault.com/questions/587727/how-to-unify-package-installation-tasks-in-ansible -- Install packages using Ansible in a Linux-agnostic way (i.e. without saying (if os==RedHat or if os==Ubuntu)). The goal is for this tool to instantiate specified number of master and node machines using Ansible and VirtualBox running a specified Linux distro. To start, this project will assume Ubuntu. 

* https://github.com/kubernetes-sigs/kubespray -- Kubespray uses Ansible to push Kubernetes to specified Linux machines. This tool will utilize Kubespray to push configure Kubernetes master and node machines running Linux on VirtualBox machines.

* https://opensource.com/resources/vagrant -- Vagrant is a tool that abstracts VM creation. The default provider is VirtualBox. But other providers such as VMWare and Docker can be used. This was found when looking up how to provision a machine using Ansible. Apparently Ansible isn't specifically used itself to provision other machines. It is used to *configure* machines that have already been provisioned. Ansible and Vagrant can work closely together, though, to achieve the goals of this project. (Ansible+Vagrant to create machines for Kube cluster, Ansible to configure machines in Kube cluster)

* https://spaceweb.nl/provisioning-a-virtual-machine-with-ansible/ -- Using Ansible+Vagrant to provision virtual machines. The author prefers VMWare, but the general concepts should be the same, since Vagrant provides an abstraction for provisioning machines.

* https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-ansible-on-ubuntu-16-04 -- Installing Ansile. Need to install Ansible on Ubuntu. *Note: The step was not followed to add the PPA repository. Only "sudo apt-get install ansible" was run.*
