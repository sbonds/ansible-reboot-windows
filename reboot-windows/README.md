Reboot Windows
=========

This sends a message to all users on the Windows target host, waits a while, then reboots the target.

Requirements
------------

Setting up WinRM on Windows is painful, but if you can get `win_ping` working, this role will probably work too.

Role Variables
--------------

warning_message: what text to send in the initial dialog
reboot_message: what text to send in the actual reboot message
advance_warning_seconds: how many seconds before the reboot to send the warning message

Dependencies
------------

No other role dependencies.

Example Playbook
----------------

```yaml
- hosts: all
  roles:
      - { role: reboot-windows }
```

License
-------

GPLv3

Author Information
------------------

Steve Bonds