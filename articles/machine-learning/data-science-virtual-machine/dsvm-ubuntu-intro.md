---
title: Provision a Linux (Ubuntu) Data Science Virtual Machine on Azure | Microsoft Docs
description: Configure and create a Data Science Virtual Machine For Linux (Ubuntu) on Azure to do analytics and machine learning.
services: machine-learning
documentationcenter: ''
author: gopitk
ms.author: gokuma
manager: cgronlun


ms.assetid: 3bab0ab9-3ea5-41a6-a62a-8c44fdbae43b
ms.service: machine-learning
ms.component: data-science-vm
ms.workload: data-services
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: conceptual
ms.date: 03/16/2018

---

# Provision the Data Science Virtual Machine for Linux (Ubuntu)
In this quickstart, you will create your Ubuntu based  Data Science Virtual Machine for Linux. For a complete listing of the data science tools  and libraries preconfigured for this DSVM please refer to the Overview.

A [CentOS](linux-dsvm-intro.md) image is also available, with many of the same tools as the Ubuntu image. A [Windows](provision-vm.md) image is available as well.

## Prerequisites
Before you can create a Data Science Virtual Machine for Linux, you must have an Azure subscription. To obtain one, see [Get Azure free trial](https://azure.microsoft.com/free/).

## Create your Data Science Virtual Machine for Linux

1. Navigate to the virtual machine listing on the [Azure portal](https://portal.azure.com/#create/microsoft-dsvm.linux-data-science-vm-ubuntulinuxdsvmubuntu). You may be prompted to login to your Azure account if you are not already signed in.  In the Search Bar type,  Data Science Virtual Machine and select Data Science Virtual Machine for Linux (Ubuntu) under Marketplace in the dropdown.

2. Click **Create** (at the bottom) to bring up the wizard.![configure-data-science-vm](./media/dsvm-ubuntu-intro/configure-data-science-virtual-machine.png)

3. The following sections provide the inputs for each of the steps in the wizard (enumerated on the right of the preceding figure) used to create the Microsoft Data Science Virtual Machine(insert updated image). Here are the inputs needed to configure each of these steps:
   
   a. **Basics**:
   
•	Subscription: If you have more than one subscription, select the one on which the machine is to be created and billed. You must have resource creation privileges for this subscription.
•	Virtual Machine Name: Name of your data science server you are creating.
•	Region: Choose the Azure region that is appropriate for you and  your customers. Not all VM sizes are available in all regions.
•	Authentication type: Choose whether the administrator account will use username/password or SSH key for authentication
1.	If you choose Password,
    User Name: First account sign-in ID.
   	Password: The administrator password for this VM
    Confirm Password: The administrator password for this VM again
2.	If you choose SSH public key,
   Username: The administrator username
   SSH public key

   
b. **Disks**:
•	Disk Options: Here you have the option to choose Premium SSD or Standard SSD  if you prefer a solid-state drive (SSD), or Standard HDD. Hover over the information icon to the right of the Disk Options for more information.
c. **Networking**:
d. **Management**:
e. **Guest Config**:
f. **Tags**:
Note: Before clicking Review+Create, be sure to review your inputs for all the previous sections of the wizard to ensure your entries are appropriate for your needs. 
g. **Review + Create**: When you’re ready, click Review+ Create and you’re on your way to creating your Data Science Virtual Machine. 
The creation of the DSVM should take about 5 minutes. Once complete the status of the provisioning is displayed on your Azure portal.

## Next steps


* How to Access the Data Science Virtual Machine for Linux (link to separate article)

* The [Data science on the Data Science Virtual Machine for Linux](linux-dsvm-walkthrough.md) walkthrough shows you how to perform several common data science tasks with the Linux Data Science VM provisioned here. 
* For a basic introduction and more information about the tools installed on the VM run *dsvm-more-info* on the shell within the virtual machine. 
* Visit the [Azure AI Gallery](https://gallery.azure.ai/) for machine learning and data analytics samples that use the Azure AI services.
* Learn how to build end-to-end analytical solutions systematically by using the [Team Data Science Process](http://aka.ms/tdsp).


