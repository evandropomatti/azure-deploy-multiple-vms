# Deploy multiple VMs in Azure
Generalizing and deploying multiple VMs in Azure

# Preparing your VM

Important: These procedures clean the OS configuration. Make a backup/snapshot first.

#### For Windows

Use System Preparation Tool.

```
sysprep /generalize
```

#### For Linux

```sh
# Take a backup of the VM first
sudo waagent -deprovision+user
```

## Template

https://github.com/Azure/azure-quickstart-templates/tree/master/201-vm-copy-managed-disks
