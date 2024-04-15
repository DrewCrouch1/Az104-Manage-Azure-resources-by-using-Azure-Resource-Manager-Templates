# Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates

## Job skills
•	Task 1: Create an Azure Resource Manager template.
•	Task 2: Edit an Azure Resource Manager template and redeploy the template.
•	Task 3: Configure the Cloud Shell and deploy a template with Azure PowerShell.
•	Task 4: Deploy a template with the CLI.
•	Task 5: Deploy a resource by using Azure Bicep.

## Task 1: Create an Azure Resource Manager (ARM) Template
### Creation of a disk to download the associated template.

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/91f82679-dd91-46c1-8069-543573953626)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/1f0051d8-1511-457c-83eb-17c444c2cadc)

## Task 2: Edit an Azure Resource Manager template and then redeploy the template
### Template Before:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/402e3caa-b2b5-4f22-893b-e90d5201545a)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/6ce49846-9882-47aa-9af4-c8d04e886323)

### Template After:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/5de1ef4d-b366-4aaa-a384-62bc16e96933)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/5c61c170-2733-47d3-b944-77c6bcf6ee80)

### Parameters Before:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/bf4ada1b-c44e-43c9-9cb8-8dfa90a957ec)

### Parameters After:
 
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/f30ab7ff-e235-44d4-a023-8a241d97f183)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/8caeb865-68db-4f8f-9393-1bef5f4f63bc)

### Deployment of the new disk from the updated ARM Template and Parameters Files

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/c1574a1a-2922-4d9c-ad7f-d0ba20989021)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/e7cef550-e5f6-43d7-9e05-280fad3e286e)

## Task 3: Configure the Cloud Shell and deploy a template with Azure PowerShell
 
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/57572aa6-d494-4365-8f99-9bf97567a6f1)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/6b26fe00-48bc-4fb2-b53b-fe5f44211b2e)

### Editing the name of the disk to “az104_disk3” in the template we previously created:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/e8ae4173-f0a8-4eae-ac1c-0eef57556043)
 
### Deploying the az104-rg3 disk via PowerShell:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/85a63903-f3e5-4139-aa70-44959bbc467e)
 
### Confirming the disk “az104_disk3” was created by using Get-AzDisk:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/1bee33e5-3fe9-4a20-91a4-c68e6747bd80)
 
## Task 4: Deploy a template with the CLI
### Editing the name of the new disk to be deployed to az104-disk4

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/5dde90b3-638f-449e-ba07-19314e25c1f8)

### Hit an error the first time trying to run this script stating the “Resource Group was not found.” I double-checked my spelling and went into the portal to verify the resource group was in fact there. I then ran “az account list --output table” and noticed my default wasn’t the subscription the resource group was in. I then used “az account set --subscription ‘subscription ID’” to switch the subscription to where the resource group was housed.
 
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/86d1da1d-5488-4cdb-9133-0b3f88f4eaad)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/ad9e3750-26ac-40ef-ad24-f103a114b3e6)

### Deployment successful:
 
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/a178e5ac-79bf-4989-a1d4-eb8a28336a83)

## Task 5: Deploy a resource by using Azure Bicep
### In Bash, uploading a bicep template and editing the name, sku and disk size:

### Before:
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/4a00c644-5c01-4719-9fe4-19eb6eec7e71)

### After:
![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/ad203c7d-5247-4cfb-944c-c888a1acd50d)

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/63c1775d-023f-4f47-84b0-8a00861aa1f7)
 
### Disk4 has been successfully provisioned via the Bicep template

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/49bc79c0-4d00-4b9d-b9df-389e45b5e395)

## Cleaning up resources via the CLI:

![image](https://github.com/DrewCrouch1/Az104-Manage-Azure-resources-by-using-Azure-Resource-Manager-Templates/assets/158229796/6672bcba-87a3-4343-9399-56fcd2139281)

