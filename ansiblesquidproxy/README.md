### Requirements

* Ansible 2.4.2.0 version 
* Ubuntu 14.04 or Ubuntu 16.04

### İnstall Ansible

```
sudo apt-get update
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

### Edit Ansible hosts

vi /etc/ansible/hosts

```
test
192.168.203.132 ##myLocalİp
```

### Ansible-playbook run

ansible-playbook --extra-vars "ip=PROXYİPADDRES" proxy.yml -kK

