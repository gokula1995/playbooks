# Setting Up ELK Cluster using Ansible
This playbook helps you to setup ELK Cluster


## Steps to run this playbook
1. Edit the ansible hosts file(/etc/ansible/hosts) and add 'elk' for the server we want to install elk.

```
[elk]
<IP> ansible_user=<User>
```
2. Run the below command to check the connectivity
```
            ansible elk -m ping
```
3. Run the below command to start the playbook
```
            ansible-playbook elk.yml
```