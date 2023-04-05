installed ansible on ansiblecontrolnode01 and validated the configuration  
created a folder called "ansible" and ansible.cfg file by creating inventory file name inventory.  
Added the private ip of homechallengedev01 to inventory.  
Generated pubkey by running ssh-keygen in ansiblecontrolnode01 and copied over to homechallengedev01 for passwordless authentication.  
created two bash file in ansiblecontrolnodedev01 security_agent_installer_linux_amd64_v1.0.0.sh and security_agent_config.yaml by copying the given code.  
Created playbook file hcplaybook.yaml to copy these file to remote server and execute it.  


#Handle sensitive data, such as the token, in a secure manner
-----------------------------------------------------------

created secrets.yml ,edited secrets.yml by adding "stoken" varibel with given value  
Encrypted the token with ansible-vault.  
During run time call the playbook with vault password  
ansible-playbook myplaybook.yaml --vault-password-file=/home/ubuntu/ansible/vaultpassword.txt  

#Ensure that the Ansible playbook can be reused against multiple systems
----------------------------------------------------------------------

Add new servers to the inventory file  


#Ensure idempotency and implement unit testing for the Ansible playbook.
-----------------------------------------------------------------------

Each execution output is writtern into output_ansibledatetime.txt and validate its successfully executed. 