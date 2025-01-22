playbook-sonarqube.yml 
- name: Apply SonarQube Role
  hosts: all
  become: yes
  roles:
    - sonarqube_role

playbook-nexus.yml 
- name: Apply Nexus Role
  hosts: all
  become: yes
  roles:
    - nexus_role

I faced this error TASK [nexus_role : Download Nexus] *************************************************************************************************************************************************************************
fatal: [localhost]: FAILED! => {"changed": false, "dest": "/tmp/nexus.tar.gz", "elapsed": 11, "gid": 0, "group": "root", "mode": "0644", "msg": "Connection failure: The read operation timed out", "owner": "root", "size": 239429340, "state": "file", "uid": 0, "url": "https://download.sonatype.com/nexus/3/latest-unix.tar.gz"}
I added "--ask-become-pass" attr
ansible-playbook playbook-nexus.yml --ask-become-pass
