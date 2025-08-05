# ansible

cd setup-harvester

# install k3s cluster

Run `ansible-playbook --inventory inventory/vm-setup-playbook/hosts setup-k3s.yaml --limit blue`

you will get the kubeconfig and cluster for you cluster on kubeconfig directory.
download the kubedb license on /Downloads directory and run the following command after downloading.

# Setup Cluster

install kubedb,kubestash,promethus,cert-manager,panopticon,metrics

`ansible-playbook --inventory inventory/vm-setup-playbook/hosts setup-cluster.yaml --limit blue`