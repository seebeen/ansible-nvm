nvm
========

Install nvm and Node.js.

Requirements
------------

git, curl, build-essential, libssl-dev. Requirements are installed by the role.

Role Variables
--------------

* `nvm.user` Remote user. Defaults to ansible `remote_user`.
* `nvm.version` nvm version tag, or `HEAD`. Defaults to `v0.4.4`
* `nvm.node_version` Node.js version. Defaults to `'8.10.'`

Dependencies
------------

No depedencies.

Example Playbook
-------------------------

    - hosts: servers
      roles:
        - role: seebeen.nvm
          nvm:
            user: deploy
            version: v0.4.4
            node_version: '8.9.4'

License
-------

GPL

Author Information
------------------

Sibin Grasic
