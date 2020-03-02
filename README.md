hyperized.docker-container
=========

_Installs docker container as a systemd service._

Notice: does not really clean up after itself (TODO)

Requirements
------------

Ansible 2.5 or above is highly recommended.

Role Variables
--------------

    docker_container_state: present
    docker_container_running_state: started
    docker_container_enabled: yes
    docker_container:


Dependencies
------------

    hyperized.docker
    hyperized.pip

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - role: hyperized.docker-container
          docker_containers:
            - name: redis

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben@hyperized.net>
