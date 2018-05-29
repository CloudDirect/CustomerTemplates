# N Tier IaaS

This master template deploys an N-tier IaaS (Infrastructure as a Service) solution to Azure. The default solution includes web, application and database tier Virtual Machines running Windows with VPN Gateway for connectivity to remote network. This template follows best practice for deploying a N-tier application, and will deploy with the specified number of VMs in each tier.

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FCloudDirect%2FMasterTemplates%2Fmaster%2Ftemplates%2Fn-tier-iaas%2Fazuredeploy.json)

## Deploy from Azure CLI

	Update Parameters in the azuredeploy.parameters.json
	
	az group deployment create --resource-group infra-prod-rg --name deployNTierIaaS --template-file n-tier-iaas/azuredeploy.json" --parameters	"@n-tier-iaas/azuredeploy.parameters.json" --no-wait


## Deploy from Azure Portal (UI Experience)

Steps:
1.  This template uses Managed Disks, there is no need to create a storage account to hold your disks.
2.  Logon to http://portal.azure.com
3.  New and search for "Template Deployment"
4.  Copy and paste the contents of azuredeploy.json into "Edit Template"
5.  Update all Parameters
6.  Follow the rest of the UI