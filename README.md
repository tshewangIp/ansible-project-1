# ansible-project

> generate ssh-keys if you don't have
>> $ ssh-keygen

> copy ssh key to target machine for passwordless login
>> ssh-copy-id -i .ssh/id_rsa.pub student@machineip
  

$ git clone https://github.com/kapilsthakkar25/ansible-project

$ cd ansible-project

$ ansible-playbook -i inventory/hosts.ini ping.yml

$ ansible-playbook -i inventory/hosts.ini site.yml

$  ansible-playbook -l lab1 -i inventory/hosts.ini site.yml -e "state=absent"

$  ansible-playbook -l lab1 -i inventory/hosts.ini site.yml -e "state=present"

$ ansible-playbook -l lab1 -i inventory/hosts.ini site.yml -e "myrepo=https://github.com/kapilsthakkar25/space-shooter"
 
$ ansible-playbook -l lab1 -i inventory/hosts.ini site.yml -e "myrepo=https://github.com/kapilsthakkar25/webapp-repo"
