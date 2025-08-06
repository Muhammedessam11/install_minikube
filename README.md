Ansible Role: install_minikube
=========

This Ansible role installs [Minikube](https://minikube.sigs.k8s.io/) and sets up a local single-node Kubernetes cluster using the Docker driver on Ubuntu systems.

Requirements
------------

- Ubuntu (20.04, 22.04, 24.04)
- Docker must be installed (the role installs it if not present)
- Make sure the target user is not `root` (Minikube does not support Docker driver as root) .

Role Variables
--------------

This role does not require any custom variables by default.


Example Playbook
----------------


    - name: Install Minikube
      hosts: localhost
      become: true
      roles:
        - install_minikube

Author Information
------------------

Name: Mohamed Essam .
Github: https://github.com/Muhammedessam11 .
Dockerhub: https://hub.docker.com/repositories/mohamedessam1911 .
