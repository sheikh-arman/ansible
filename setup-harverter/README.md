# ansible

cd setup-harvester

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml`

# runtime variable

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --limit blue`