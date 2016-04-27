Role Name
=========
[![license][2i]][2p]
[![twitter][3i]][3p]

Install tup from source.

Description
-----------

[Tup][4] is a DAG file based build system. Pretty darn great for a number of automation build setups. This role here installs [tup][4] from the [git][5] repository.

Role Variables
--------------

You only need to change one variable **dir.tool** in `defaults/main.yml`. The variable is where you will have the tup build installed.

Requirements
------------

Due to build necessities, the module requires to have [abaez.common][6] installed for the prerequisites for the build to be successful.

Usage
-----

All you need is to have [abaez.common][6] and you should be good to go to run the role:

``` yaml
- hosts: servers
    roles:
        - abaez.common
        - tup
```

Author Information
------------------

[Alejandro Baez][1]

[1]: https://keybase.io/baez
[2i]: https://img.shields.io/badge/license-BSD_2-green.svg
[2p]: ./LICENSE
[3i]: https://img.shields.io/badge/twitter-a_baez-blue.svg
[3p]: https://twitter.com/a_baez
[4]: http://gittup.org/tup
[5]: https://github.com/gittup/tup
[6]: https://galaxy.ansible.com/abaez/common
