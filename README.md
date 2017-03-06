## Standalone Mongodb Deployment to ubuntu Os

- Requires Ansible 1.2 or newer
- Expects Ubuntu hosts
- Install mongodb 3.0 or latest


This playbook deploys an implementation of mongodb Server,
3.0 or the latest. To use them, first edit the "hosts" inventory file to contain the
hostnames of the machines on which you want mongodb deployed, and edit the
group_vars/mongodb-servers file to set any mongodb configuration parameters you need.

Then run the playbook, like this:

	ansible-playbook -i hosts --user=ubuntu site.yml 

	
When the playbook run completes, you should be able to see the mongodb
running on the target machines.

