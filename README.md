Setup Ansible on ansible controller machine with following commands

yum update
yum install ansible -y

Since the finalproject playbook uses community modules from ansible galaxy you will need to install it using the following command

ansible-galaxy collections install community.mysql

To run the playbooks use the command with following syntax

ansible-playbook <playbookname> -i inventory finalproject

NOTE: This is ansible practice repository. The information in the inventory are setup to use the virtual machines created in a virtual box in the same network. The passwords are also kept in the playbook as well as the inventory files to practice basic ansible. They will be moved to vaults as I learn more about ansible.
