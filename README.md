## Ansible Playbooks to deploy Converged Infrastructure stack in Intersight Managed Mode (IMM)

### Workflows

Converged Infrastructure stack in Intersight Managed Mode is deployed in multiple phases. It involves below steps in order.

1. Configure UCS Domain Policies
2. Configure UCS Domain Profiles
3. Deploy UCS Domain Profile
4. Configure pools like MAC, IP, WWN, IQN
4. Configure UCS Server Policies
5. Configure UCS Server Profiles
6. Associating profiles to physical servers.

<br />
<br />
<br />

### Summary of steps to deploy server profiles.
1. Updates all the required input in the folder **Input_Required**
2. Create Pools. 
   Run:  **ansible-playbook create_pools.yaml **
4. Create Policies. 
   Run:  **ansible-playbook create_pools.yaml **
6. Create and deploy server profiles.
   Run:  **ansible-playbook deploy_server_profiles.yaml **
