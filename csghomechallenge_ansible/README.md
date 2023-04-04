# installed ansible on ansiblecontrolnode01 and validated the configuration
# created a folder called "ansible" and ansible.cfg file by creating inventory file name inventory.
# Added the private key ip of homechallengedev01 to inventory.
# Generated pubkey by running ssh-keygen in ansiblecontrolnode01 and copied over to homechallengedev01 for passwordless authentication.
# created two bash file in ansiblecontrolnodedev01 security_agent_installer_linux_amd64_v1.0.0.sh and security_agent_config.yaml by        
  copying the given code.
# Created playbook file hcplaybook.yaml to copy these file to remote server and execute it.
# run the play book ansible-playbook -i inventory hcplaybook.yaml
# check the output.txt file and validate the script executed successfully.
