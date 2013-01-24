SEFix
=====

Description
-----------
Simple script to respond to SELinux AVC Denials

Usage
-----
    # ./sefix [searchname]

Examples
--------
    # ./sefix vsftpd
    # ./sefix sshd

Process
-------
Sefix will search for the passed option in /var/log/audit.log. If it successfully finds a denial it will generate a policy file and use semodule to install it.

Prerequisites
-------------
policycoreutils

