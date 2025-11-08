# Projet Vagrant + Ansible

Ce projet crée une VM Ubuntu avec Vagrant et installe automatiquement Ansible.  
Un playbook installe Apache sur la machine.

## Étapes
1. `vagrant up` — lance la machine virtuelle.  
2. `vagrant ssh` — se connecter à la VM.  
3. `cd /home/vagrant/ansible` — accéder au dossier Ansible.  
4. `ansible-playbook playbook.yml` — exécuter le playbook.
