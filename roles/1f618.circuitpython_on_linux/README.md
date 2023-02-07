Role Name
=========

This role installs CircuitPython on Linux, based on the [Adafruit guide](https://learn.adafruit.com/circuitpython-on-raspberrypi-linux/installing-circuitpython-on-raspberry-pi) by [Melissa LeBlanc-Williams](https://learn.adafruit.com/u/MakerMelissa).

Requirements
------------

None.

Role Variables
--------------

`blinka_dir` is set in vars/main.yml, and defaults to `~/blinka_install`.

Dependencies
------------

`geerlingguy.pip`

Example Playbook
----------------

```
---
- hosts: pi
  roles:
      - { role: 1f618.circuitpython_on_linux }
```

License
-------

MIT

<!-- Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed). -->
