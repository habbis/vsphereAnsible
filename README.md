# vsphereAnsible
Ansible playbook for provisioning vm via [vmware vsphere module](https://docs.ansible.com/ansible/latest/modules/vmware_guest_module.html) 

First you setup a template on your vcenter.

To setup a vm 
```
ansible-playbook site.yml
```
Then running this playbook you will use host localhost since 
the ansible module will connect with parameter supplied in the task.

I have created standalone playbook for deprovisioning 
```
ansible-playbook removingVM.yml     
```

All the variabels are in [group_vars](/group_vars/all) folder. 

To encrypt passord and username you can use [ansible vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html) .

