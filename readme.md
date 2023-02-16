# azure-cli-install


This is a simple ansible playbook, that is used for **Azure CLI** installation, acording to [this page](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-linux?pivots=apt).

Verified on:
* Ubuntu-22.04
* kali-linux

### Pre-requirements

[Ansible](#install-ansible) must be installed.

### Usage

1. `cd` into project directory.
2. Execute:

    ```bash
    ansible-playbook azure_cli_install.yaml -K
    ```
    * `-K` - provide *sudo* password for ansible *privilege escalation*

### Install Ansible

* Update repos list:

    ```bash
    sudo apt-get update
    ```

* Install Ansible:

    ```bash
    sudo apt-get install ansible -y
    ```
    * `-y` - assume "yes" as answer to all prompts and run non-interactively


---
