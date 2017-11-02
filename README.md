clean-container-cache
=========

Slim your Ansible Container images by cleaning out apt, pip, and/or yum package caches.

Though this behavior is usually only desirable when building container images, this role should work just as well to clean out the package cache on virtual machines.

Role Variables
----------------

* `pip_cache_dir: "{{ ansible_env.HOME }}/.cache/pip"` 
  * Absolute path of the pip cache

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - marcusianlevine.clean-container-cache
```

License
-------

BSD

Author Information
------------------

Written by Marcus Levine.
