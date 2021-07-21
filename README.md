aws-corretto
=========

This role installs AWS Corretto 8, for unix-like platforms.

Requirements
------------
- sudo permission 

Role Variables
--------------

You need to pass required versions and platforms as variables before/ during runtime.
| Variable               |Default                          |Available Values                          |
|----------------|-------------------------------|-----------------------------|
|corretto_base_url               |https://corretto.aws/downloads/resources|https://corretto.aws/downloads/resources|
|corretto_major_version          |8                                       |8/11/15      |
|corretto_minor_version          |275.01.1                                |as updated|
|corretto_platform               |linux-x64                               |linux-x64/Linux aarch64


Dependencies
------------
- git must be installed
- Ansible must be installed


Steps
----------------
1. Update your variables with required version
2. Clone the repository
3. Switch to the repository and below command
    ```sudo ansible-playbook -i localhost site.yml```

References
-------
Source : https://github.com/corretto/corretto-8/releases

