Playbooks from this folder are for setting up server and installing [XMD](https://github.com/sseshachala/xmd)

Install
=======

No special dependincies

Usage
=====
```
export ANSIBLE_HOST_KEY_CHECKING=False

cd xmd_dev
 
ansible-playbook xmd.yml -i hosts -u root -k 
```
