# Install docker using Ansible to CentOS7
Connect to your Ansible machine and follow the steps bellow
```
git clone https://github.com/farkhodsadykov/docker-install.git
cd docker-install
```

Pleas before running the ansible-playbook change the hosts file add your servers ip. Then ssh-copy-id as root or user which has sudo permission.
```
ssh-copy-id root@yourserversip
```

## Verify
```
ansible all -u root -i hosts -m ping
```

## Installing docker to remote machine 
```
ansible-playbook -u root -i hosts docker-install-ce.yml
```


Thank you :) 
