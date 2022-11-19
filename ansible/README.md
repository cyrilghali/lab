# Ansible Cheetsheet

## Setup an inventory and test it

Setup your inventory:
```sh
sudo vim /etc/ansible/hosts
```

Put this snippet
```
[example]
www.example.com
www.example2.com
```

Run this ad-hoc command to test it
```
ansible example -m ping -u username
```
