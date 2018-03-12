# Ansible KnowHow

## Playbooks and beginner things...

### Basic ping
-  ansible -i ./hosts web -m ping

### get output of "ip addr" from hosts
- ansible-playbook -i hosts pb/get_ip.yml
