# kubeadm-deployment-unleashed
Automating &amp; customizing K8s deployment using Kubeadm "phases" (or not).

**Work in progress**

## Prequisites
This project assumes that your networking "underlay" is already working.
(If it doesn't, feel free to use this project : https://github.com/jpmondet/FullyAutomatedBGPfabric)

## How-to

From your ansible admin machine : 
```bash
git clone https://github.com/jpmondet/kubeadm-deployment-unleashed.git
```

**Review the variables in host_vars/global_vars.yaml to match your needs**
You can choose the networking options/plugins and even to add Istio automatically.
TODO: explain all the variables/choices (there are already explanations in the variables yaml file.)

Then : 

```bash
cd kubeadm-deployment-unleashed
ansible-playbook deploy_kubeadm.yaml
```


You are now good to go to play with your new kubernetes cluster ! 