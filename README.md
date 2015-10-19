# ansible-ssh-update-keys
Ansible playbook for adding or remove ssh keys under 1 user account

1. in the hosts file, specifiy the group of servers you'd like to configure (in this example I have 2 application servers and 1 database server)
2. To add new user's key add the user's pub key inside the folder "keys_to_add"
3. To remove user's key, move the user's pub key into the folder "keys_to_drop"
4. Run the playbook: ```$ansible-playbook update_keys.yml```
