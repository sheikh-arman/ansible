# ansible

cd setup-harvester

# install k3s cluster

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts k3s.yaml --limit blue`

# Setup Cluster

install kubedb,kubestash,promethus,cert-manager,panopticon,metrics

`ansible-playbook --inventory inventory/vm-setup-playbook/hosts setup-cluster.yaml --limit blue`