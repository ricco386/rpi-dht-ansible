Ansible rpi-dht role
====================

Ansible role for installing RPi.DHT sensor (https://github.com/ricco386/RPi.DHT).

Requirements
------------

RPi.DHT is Raspberry Pi specific library, role can be sucessfuly run only ar Raspberry Pi.

Role Variables
--------------

Development version, whether to clone GIT repo for later development as well?
        rpi_dht_dev: False

Sensor configuration variables
        rpi_dht_config: /root/.sensor.cfg
        rpi_dht_config_node_id: 1
        rpi_dht_config_hostname: False
        rpi_dht_config_username: False
        rpi_dht_config_password: False

Tries to start and enable service sensor once everything is installed.
        rpi_dht_service: True

Generic user that is used on RPi
        rpi_dht_username: pi


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: raspberrys
      roles:
        - { role: rpi-dht , rpi_dht_dev: True }

License
-------

MIT

Author Information
------------------

Richard Kellner
