#### How to create an Ansible Configuration  
1. First allow direct root access via SSH with another server's IP (ex.: ssh root@ip), after that, go back to alpine user.  
2. Install ansible and sshpass dependencies and packages. (commands: apk add ansible and apk add sshpass)  
3. Configure the control node user for passwordless super user access.  
4. Create an ansible configuration file (ex. ansible.cfg)  
5. Insert basic information such as inventory, host verification, and default remote user.  
6. Save the file.  
#### How to create Ansible Inventory.  
1. Create an inventory file with the same name inside the defaults in configuration file, to do this use vim. (ex. vim inventoryfiles)  
2. Obtain information about your ansible inventory, you can add here the Ubuntu's IP address.  
3. Save the file.  
#### How to create an Ad-hoc Ansible command with setup and shell module.  
1. Connect using "ping" module via adhoc command. (command: ansible all -m ping), this will execute the ping module on all hosts listed in your custom inventory file.  
2. If unreachable, you can use the command: ansible -m ping -k.  

