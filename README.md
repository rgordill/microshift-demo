# Edge Microshift Builder

This project provides Ansible roles and tasks to automate the creation and management of KVM-based virtual machines for edge computing environments. It includes playbooks for provisioning VM disk images, configuring permissions, and preparing VMs based on RHEL9 images.

# Vault

Not included in this repo, a vault.yml is also needed. It contains:

- `ansible_become_pass`: Password used by Ansible for privilege escalation in localhost for KVM.
- `org_activationkey`: Activation key for registering systems with your organization's Red Hat subscription.
- `org_id`: Organization ID for subscription or registration purposes.
- `password`: Generic password used for VM or system user accounts.
- `ssh_public_key`: SSH public key to be injected into the VM for secure access.
- `pull_secret`: Secret used to authenticate and pull container images from protected registries.