# Docker role for Ubuntu 14.04

This follows docker installation for ubuntu 14.04 explained in
[the official documentation](https://docs.docker.com/engine/installation/linux/ubuntulinux/).

Role Variables
--------------

You can specify user to be included in docker group,
which makes user able to run docker commands without `sudo`.

For example:

```
---
docker-group:
  - ubuntu
  - deployer
```

Example Playbook
----------------

Tested with:

```
$ ansible --version
ansible 2.1.0 (devel 50dfd4b057) last updated 2016/02/07 13:39:55 (GMT +900)
  lib/ansible/modules/core: (detached HEAD e1ec52e365) last updated 2016/02/07 13:41:53 (GMT +900)
  lib/ansible/modules/extras: (detached HEAD 14a62fb5d6) last updated 2016/02/07 13:42:45 (GMT +900)
  config file =
  configured module search path = Default w/o overrides
```

Example is here [hi-ogawa/ansible-role-docker-example](https://github.com/hi-ogawa/ansible-role-docker-example).

License
-------

BSD
