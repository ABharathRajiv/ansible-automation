# Ansible Playbooks for HAProxy Management and Kernel Configuration

This Git repository contains Ansible playbooks to automate the management of HAProxy, configure kernel parameters, and update HAProxy configurations. These playbooks are designed to streamline the process of deploying and maintaining HAProxy instances with specific configurations and kernel settings.

## Requirements

Before using these Ansible playbooks, ensure that you have the following prerequisites:

- Ansible installed on the machine where you will run the playbooks.
- Proper SSH access to the target machines where HAProxy is installed.
- Access to modify kernel parameters on target machines.

### Playbooks
    -start_hap.yml
    -stop_hap.yml
    -restart_hap.yml
    -set_hap_params.yml
    -configure_hap.yml

### HAProxy Management

The repo's playbook provides functionality for starting, stopping, restarting, configuring and setting kernel parameters in the HAProxy service on target machines.

The host details is defined in the environment/inventory

### To run the playbook.
```
Setup Ansible-vault using : ansible-vault create vaultfilename.yml

```
```
ansible-playbook --ask-vault-pass -i environment/inventory playbookname.yml
```
### Ansible log
The log file is stored in log directory along with error-log
