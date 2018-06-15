#  Ansible Role: Jenkins

Installs Jenkins on RHEL/CentOS and Debian/Ubuntu servers.

## Role Variables

Available variables are listed below, along with default values (see `vars/main.yml`):

    jenkins_hostname: localhost

The system hostname; usually `localhost` works fine. This will be used during setup to communicate with the running Jenkins instance via HTTP requests.

    jenkins_jar_location: /opt/jenkins-cli.jar
    
The location at which the `jenkins-cli.jar` jarfile will be kept. This is used for communicating with Jenkins via the CLI.

Jenkins plugins to be installed automatically during provisioning. You can always install more plugins via the Jenkins UI at a later time, but this is helpful in getting things up and running more quickly.
Jenkins plugins are defined in defaults.

## Dependencies

  - osm_java
  
## Example Playbook

---
- hosts: all
  roles:
    - rolename
  become: yes
  
  
## License

MIT / BSD

## Author Information

###### www.opstree.com

