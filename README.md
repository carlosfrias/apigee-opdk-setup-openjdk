Apigee OPDK Setup OpenJDK
=========

This roles setups up the OpenJDK system packages. This role also adds Java to the default environment variables for all 
users. This role manages setting up either 1.7 or 1.8. 

Requirements
------------
The installation of Apigee OPDK requires root access. Credentials must also be supplied to override the empty placeholders
provided here. It is recommended that credentials be consolidated into a single credentials.yml file that can be stored 
separately. It is assumed that files containing credentials are stored in the ~/.apigee folder. 


Role Variables
--------------

Variables are managed in the opdk-setup-default-settings role. 

JDK Version to install

    jdk_version: '1.8'

Dependencies
------------

This role depends on the following roles: 

* opdk-setup-default-settings 

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: opdk-setup-openjdk }

License
-------

Apache License Version 2.0, January 2004

Author Information
------------------

Carlos Frias
