Playbooks from this folder are for setting up server and installing [XMD](https://github.com/sseshachala/xmd), graphios, xervrest

Install
=======

No special dependincies

Usage
=====
xmd.yml will install everything except graphite
graphite.yml will install only graphite
```
export ANSIBLE_HOST_KEY_CHECKING=False

cd xmd_dev
```

Deploying all
=============

Hosts file and vars in group_vars/all should be configured
After use command for installing both:

```
ansible-playbook deploy.yml -i hosts -u root -k 
```

or you can use to install xmd, xervrest, graphios
```
ansible-playbook xmd.yml -i hosts -u root -k 
```
for graphite
```
ansible-playbook graphite.yml -i hosts -u root -k 
```
