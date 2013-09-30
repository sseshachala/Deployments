Deployments
===========

Builds a Deployment Framework for Cloud.


Install
=======
```
 sudo apt-get install python-setuptools python-dev build-essential git sshpass
 sudo easy_install pip
 sudo pip install --upgrade virtualenv 
```
We use [custom version](https://github.com/Xervmon/ansible/tree/xervmon) of ansible based on 1.3.2 release

```
pip install  git+git://github.com/Xervmon/ansible.git@xervmon
```

Ansible Playbooks
=================

[ec2](ec2) contain playbooks for testing ec2. See [ec2 Readme](ec2/README.md)
