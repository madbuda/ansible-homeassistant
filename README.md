homeassistant
=============

Sets up and configures [Home Assistant](https://home-assistant.io/). Tested on
[Raspbian](https://www.raspbian.org/), feel free to open a PR with support for
other platforms.

Role Variables
--------------

Whether or not to enable ZWave support.

    enable_zwave: no

The contents of the Home Assistant `configuration.yaml` file.

    hass_configuration: ''

Example Playbook
----------------

    - hosts: all
      roles:
         - role: mechaxl.homeassistant
           enable_zwave: yes
           hass_configuration: "{{ lookup('file', 'configuration.yaml') }}"

License
-------

LGPL

