Install
=======

You need xervmon version of ansible installed as described in [README](../README.md)

There is boto requirements for this tasks. In order to install run
```
pip install boto
```

Ec2 tasks
=========


All tasks are stored in roles. You can run test using:

```
ansible-playbook -i dev.inventory <yml-file>
```

Vars
====

All vars are stored in [vars/amazon_creds.yml](vars/amazon_creds.yml) .
You can change to test other cases

Inventory (test host group) file is [dev.inventory](dev.inventory)

Testing
=======

All yml files stored in root of this directory are tests and can be run using as example:

```
ansible-playbook -i dev.inventory group_test.yml
```
