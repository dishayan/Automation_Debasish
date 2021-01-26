# Automation_Debasish
# Prerequisites:

(1) Here i am using root user to login to CentOS host so make sure root user should be password less login. If we are not using root 
user then we can use any other normal user with sudo privilege. In that case we have to add below two conditions in the ansible 
playbook file.

- hosts: centoshost
  remote_user: root
  become: yes  <---------------
  
  become_method: sudo  <---------------
   
(2) We are updating the CentOS so make sure the repo file should be updated properly pointing to internal repo server.
