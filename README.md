# ansible Install
sudo apt update

sudo apt install ansible -y

# ansible
cd ansible-handlers

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml`


# runtime variable
Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --extra-vars '{"version":"1.0","other_variable":"foo"}'`

# Deployment Strategy

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --limit blue`

https://github.com/rahulwagh/ansible-examples





















