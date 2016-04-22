aws-credentials
=========

Install aws credentials onto a destination machine.  ~/.aws/credentials is the location for boto and other system libraries to look for credentials.

There are two ways that credentials are obtained to put on the machine.

** Explicitly with the following variabile **

* aws_credentials_access_key 
* aws_credentials_secret_access_key

** Implicitly using a source AWS profile that is setup on the host. **

* aws_credentials_profile_source
* aws_credentials_profile_destination

Requirements
------------

For testing requires aws configure to have been run on the host machine. 

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

