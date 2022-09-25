Vector Ansible Role
=========

Устанавливает [vector](https://vector.dev) на минималках
* в Vector настраивается минимальный поток stdin->console в виде текста


Requirements
------------

N/A


Role Variables
--------------

* `vector_version` определяет версию Vector
* `vector_arch` позволяет переопределить архитектуру процессора целевого хоста


Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: dborchev.vector-role

License
-------

BSD

Author Information
------------------
N/A