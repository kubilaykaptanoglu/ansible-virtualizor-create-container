# Virtualizor create contoiner with ssh


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

### ansible-playbook run

```
ansible-playbook paket1.yml --extra-vars "id=232"  --extra-vars "ip=192.168.203.123"  --extra-vars "os=ubuntu-14.04-x86_64"  --extra-vars "hostname=test.me"  --extra-vars "user=root"  --extra-vars "password=deneme123" -kK
```

### NOTE

* id = container id
* ip= container ip address
* os = Operation System
* hostname = container hostname
* user = container login  ssh username
* password = container login  ssh password

> Create container properties 
* 512 MB RAM
* 20 GB DİSK
* 1 CORE CPU
* Unlimited traffic
