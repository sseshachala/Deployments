Install pyrax (rackspace API needed)

```
pip install pyrax
```

This repo currently has two options for creating and deleting servers. One option is to issue the request via the command line like this:

ansible-playbook -v -i dev.inventory --extra-vars "name=raxtest1 flavor=2 image=d919d2a7-5a39-48a3-be49-8c808ab4ad23 region=DFW state=deleted" site-cli.yml

The other option is to put this information in /vars/sites_enabled.yml and /vars/sites_deleted.yml like this:

servers_enabled:
  - {
      name: "raxtest1",
      flavor: "2",
      image: "d919d2a7-5a39-48a3-be49-8c808ab4ad23",
      region: "DFW"
    }
  - {
      name: "raxtest2",
      flavor: "2",
      image: "d919d2a7-5a39-48a3-be49-8c808ab4ad23",
      region: "DFW"
    }

Then issue this command:

ansible-playbook -v -i dev.inventory site-vars.yml
