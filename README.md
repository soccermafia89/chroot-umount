Role Name
=========

Umounts a boot and root device as a filesystem mount on /mnt.  Reverses what the chroot-mount role does.

Requirements
------------

None

Role Variables
--------------

- boot_device_name -- Boot device name, available on /dev/.
- root_device_name: -- Root device name, available on /dev/.

Dependencies
------------

Example Playbook
----------------

```
- name: Mount Chroot
  hosts: localhost
  roles:
   - chroot-mount
  vars:
    boot_device_name: "sdc"
    root_device_name: "sdd"
```

License
-------

BSD

Author Information
------------------

Alex Ethier, the Mitre Corporation.
