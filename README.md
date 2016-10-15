homeassistant
=============

Sets up and configures [Home Assistant](https://home-assistant.io/).

Role Variables
--------------

    enable_zwave: no

Whether or not to enable ZWave support.

    hass_configuration: ''

The contents of the Home Assistant `configuration.yaml` file.

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

