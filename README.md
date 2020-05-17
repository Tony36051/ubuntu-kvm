# bandwagon-ubuntu
Ansible deploy script for my openvz bandwagon(ubuntu 16.04)

```
#!/bin/bash

wget https://bootstrap.pypa.io/get-pip.py
python get-pip.py
sudo pip install -U ansible

sudo apt update
sudo apt install -y git
git clone https://github.com/Tony36051/bandwagon-ubuntu.git
cd bandwagon-ubuntu
ansible-galaxy install jgeusebroek.mariadb
ansible-playbook site.yml -e sspassword=123
```
# ubuntu-kvm
