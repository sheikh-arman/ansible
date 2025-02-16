# ansible
cd ansible-handlers
Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml`

# runtime variable
Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --limit blue`