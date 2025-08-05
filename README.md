# ansible Install
sudo apt update

sudo apt install ansible -y


# Install k3s and install KubeDB, kubestash 

cd setup-harvester

change the ip for your host in ./inventory/vm-setup-playbook/hosts

# install k3s cluster

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts setup-k3s.yaml --limit blue`

# Setup Cluster

install kubedb,kubestash,promethus,cert-manager,panopticon,metrics

update the version in my_vars.yml

`ansible-playbook --inventory inventory/vm-setup-playbook/hosts setup-cluster.yaml --limit blue`

# ansible
cd ansible-handlers

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml`


# runtime variable
Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --extra-vars '{"version":"1.0","other_variable":"foo"}'`

# Deployment Strategy

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts vm-setup-playbook.yaml --limit blue`

https://github.com/rahulwagh/ansible-examples





















