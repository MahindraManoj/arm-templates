# arm-templates

This repository contains custom ARM templates needed that can be used to provision resources such as Vnet, Windows VM(s), Ubuntu VMs, multiple windows server VMs with shared disks in an azure subscription.

**Prerequisites for the templates to work are below:**

- An Azure subscription
- A resouce group
- A virtual network with enough Ips available

For the VirtualNetworkDeploy template, only an azure subscription and a resource group should be present while deploying the template

**MultiWin2019VmMultiDataDiskLBDeploy**

This folder has the json code that provisions multiple Windows 2019 DC VMs within an availability set. It also deploys a basic internal load balancer and places the VMs behind the load balancer (as backend addresses). Click the below button to deploy this to Azure.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FMultiWin2019VmMultiDataDiskLBDeploy%2Fwinvmslbdeploy.json)

**UbuntuVMDeploy**

This folder contains the json code that will provision an Ubuntu 18.04 LTS VM with size Standard_B2ms. To deploy this, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FLinuxVMDeploy%2Fazuredeploy.json)

**MultiWin2019VmMultiDataDiskDeploy**

This folder contains the json code to provision mutiple windows server 2019 DC edition VMs with Mutiple Data Disks attached to each VM. To deploy the template, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FMultiWin2019VmMutilDataDiskDeploy%2Fazuremultivmsdeploy.json)

**MultiWin2019VmMultiSharedDiskDeploy**

This contains the json code to provision  mutiple windows server 2019 DC edition VMs with mutiple data disks shared between the VMs.

Prerequisite:

- Understand how shared disk concept works before if not familiar with it.
- The mazShares property for the data disks that will get created has been set to 2. If the disk(s) need to be shared with more than 2 VMs, then the value needs to be changed accordingly.

To deploy this template, click the below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FMutilWin2019VmMultiSharedDiskDeploy%2Fazuredeploy.json)

**VirtualNetworkDeploy**

This template creates a virtual network (and a subnet). To deploy, click below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FVirtualNetworkDeploy%2Fazuredeploy.json)

**WinServerVmDeploy**

This template provisions either a Win 2016 Data Center VM or a Win 2019 Data Center VM. It can have data disk(s) attached to it if needed. To deploy this, click below button.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FMahindraManoj%2Farm-templates%2Fmaster%2FWin2019VmDeploy%2Fazuredeploy.json)





