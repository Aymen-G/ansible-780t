Role edcs.docker
=========

Ce rôle permet l'installation de docker et, au choix, de docker-compose; 


Requirements
------------

Pas de conditions préalables ou package requis, connus à ce jour

Role Variables
--------------

docker_no_proxy: ne pas passer par le proxy   (localhost,127.0.0.1)
docker_dockerd_args: argument de dockerd (-H fd://)
docker_docker_conf: dictionnaire contenant la conf de docker deamon  {}
docker_namespace_group: groupe de namespace docker  ("dockremap")
docker_namespace_user: user de namespace docker  ("dockremap")
docker_id_remap: numéro ID : (296608)
docker_userns_remap: variable de docker remap  ()


Dependencies
------------

Le rôle dépend du rôle : geerlingguy.docker

Example Playbook
----------------

Exemple:

    - hosts: servers
      become: yes
      roles:
      - edcs.docker

 

License
-------

EDCS

Author Information
------------------

Said ACHBAKOU
