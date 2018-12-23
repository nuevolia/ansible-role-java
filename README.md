# Ansible Role: Java

[![Build Status](https://travis-ci.org/nuevolia/ansible-role-java.svg?branch=master)](https://travis-ci.org/nuevolia/ansible-role-java)

Installs Java for RedHat/CentOS and Debian/Ubuntu linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    # The defaults provided by this role are specific to each distribution.
    java__packages:
      - java-1.7.0-openjdk

Set the version/development kit of Java to install, along with any other necessary Java packages. Some other options include are included in the distribution-specific files in this role's 'defaults' folder.

    java__java_home: ""

If set, the role will set the global environment variable `JAVA_HOME` to this value.

## Dependencies

None.

## Example Playbook (using default package, usually OpenJDK 7)

    - hosts: servers
      roles:
        - role: nuevolia.java

## License

MIT / BSD

## Author Information

This role was created in 2018 by [Fabien Zarifian](https://www.nuevolia.com/)

Ideas from Jeff Geerling and Maciej Delmanowski
