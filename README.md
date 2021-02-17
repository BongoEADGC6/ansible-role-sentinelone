Role Name
=========

An ansible role to install SentinelOne's antivirus agent on Linux us..

Requirements
------------

You will require a server in which to serve the rpm or deb package for any
servers or workstations that you plan to install this.

Role Variables
--------------

`sentineone_install` - Set to true to allow installation of the agent. This is good for 
controlling installs per group or hostname (Default: false)
`s1_install_dir` - Directory to install the SentinelOne agent (Default: /opt/sentinelone)
`s1_daemon` - Name for the service daemon for each Operating system
`s1_package` - Name for the temporary file that is added to the host for
installation


Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bongoeadgc6.sentenielone, 
              s1_package_url: "http://hostname/sentinelagent.rpm" }

License
-------

BSD

