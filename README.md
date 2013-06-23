My Ansible config
=================

This is my [ansible](http://ansible.cc) setup to maintain my home servers.


Installation
============

    ```
    pip install -r requirements.txt
    ```


Common usages
=============

    ```
    # Run playbook in check mode and see modified files
    ansible-playbook -DC site.yml
    # Run playbook and see modified files
    ansible-playbook -D site.yml
    # Run only unbound and dnsmasq playbooks
    ansible-playboox -D site.yml --tags="unbound,dnsmasq"
    # apt-get upgrade
    ansible all -m apt -a "upgrade=dist"
    ```
