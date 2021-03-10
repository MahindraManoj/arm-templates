# arm-templates

This repository contains custom ARM templates needed that can be used to provision resources such as Vnet, Windows VM(s), Ubuntu VMs, multiple windows server VMs with shared disks in an azure subscription.

# Prerequisites for the templates to work are below:

1. An Azure subscription
2. A resouce group
3. A virtual network with enough Ips available

For the VirtualNetworkDeploy template, only an azure subscription and a resource group should be present while deploying the template

# LinuxVMDeploy

This folder contains the json code that will provision an Ubuntu 18.04 LTS VM with size Standard_B2ms. To deploy this, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FLinuxVMDeploy%2Fazuredeploy.json)

# MultiWin2019VmMutilDataDiskDeploy

This folder contains the json code to provision mutiple windows server 2019 DC edition VMs with Mutiple Data Disks attached to each VM. To deploy the template, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FMultiWin2019VmMutilDataDiskDeploy%2Fazuremultivmsdeploy.json)

# MutilWin2019VmMultiSharedDiskDeploy

This contains the json code to provision  mutiple windows server 2019 DC edition VMs with mutiple data disks shared between the VMs.

Prerequisite:

1. Understand how shared disk concept works before if not familiar with it.
2. The mazShares property for the data disks that will get created has been set to 2. If the disk(s) need to be shared with more than 2 VMs, then the value needs to be changed accordingly.

To deploy this template, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FMutilWin2019VmMultiSharedDiskDeploy%2Fazuredeploy.json)

# VirtualNetworkDeploy

This template creates a virtual network (and a subnet). To deploy, click below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FVirtualNetworkDeploy%2Fazuredeploy.json)

# WinVMDeploy

This template provisions either a Win 2016 Data Center VM or a Win 2019 Data Center VM. It can have data disk(s) attached to it if needed. To deploy this, click below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FWin2019VmDeploy%2Fazuredeploy.json)





