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

Variables are managed in the apigee-opdk-setup-default-settings role. 

JDK Version to install

    jdk_version: '1.8'

Dependencies
------------

This role depends on the following roles: 

* apigee-opdk-setup-default-settings 

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: apigee-opdk-setup-openjdk }

License
-------

Apache License Version 2.0, January 2004

Author Information
------------------

Carlos Frias
<!-- BEGIN Google Required Disclaimer -->

# Not Google Product Clause

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
<!-- BEGIN Google How To Contribute -->
# How to Contribute

We'd love to accept your patches and contributions to this project. Please review our [guidelines](CONTRIBUTION.md).
<!-- END Google How To Contribute -->
