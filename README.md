# Ansible KnowHow

## Playbooks and beginner things...

### Basic ping
-  ansible -i ./hosts web -m ping

### get output of "ip addr" from hosts
- ansible-playbook -i hosts pb/get_ip.yml

### Do an apt-get update on remote host
- ansible-playbook -i hosts pb/apt_get__update.yml

In order to use it the most optimized way, it seems the best underlaying package is: 
aptitude (apt-get install aptitude) 
You can install it remote via:
- ansible-playbook -i hosts pb/install_aptitude.yml


### Perhaps something necessary to prevent stupid questions:
- export ANSIBLE_NOCOWS=1

