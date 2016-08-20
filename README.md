# Update the Katello Agent to 6.2

## Description

Upgrading Red Hat's Satellite 6.1.9 to version 6.2 requires all of the client
machiens to upgrade their version of katello-agent.  This is fairly simply, but
very tedius to do on a large number of machines. Perfect for a simple ansible
play.

## Cloning

This repository uses git submodules.  To grab them all, clone it with the
`--recursive` flag.

```
git clone --recursive https://github.com/chrispoupart/ansible-play-katello_agent-upgrade.git
```

## Inventory

We make use of [foreman ansible inventory](https://github.com/theforeman/foreman_ansible_inventory) 
script.  You should read their 
[documentation](https://github.com/theforeman/foreman_ansible_inventory/blob/master/README.md) 
to configure it properly for your environment.
