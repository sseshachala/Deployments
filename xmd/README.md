Playbooks from this folder are for setting up server and installing [XMD](https://github.com/sseshachala/xmd)

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
 
ansible-playbook xmd.yml -i hosts -u root -k 
ansible-playbook graphite.yml -i hosts -u root -k 
```
