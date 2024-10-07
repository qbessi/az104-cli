# AZ104 PowerSHell Command Dump
A PowerShell command dump used for the AZ-104 exam.

## Azure PowerShell Commands

### Subscription Management Commands

| Command                                      | Explanation                                                                                                                                       |
|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| `Get-AzSubscription`                         | Retrieves a list of all subscriptions associated with your Azure account. This command provides details such as the subscription ID, name, and state. |
| `Select-AzSubscription -SubscriptionId <ID>`| Sets the specified subscription as the current active subscription for the session, allowing subsequent commands to operate within that context.   |
| `Get-AzContext`                             | Displays the current Azure context, including the active subscription and tenant details. Useful for confirming which subscription you're working in.  |
| `Get-AzAccount`                             | Lists all accounts associated with your Azure environment, including subscription information. This command helps verify which subscriptions you can access. |
| `Get-AzRoleAssignment -Scope <Scope>`      | Retrieves role assignments at the specified scope (such as a subscription). This helps you understand who has access to resources in that subscription. |

### Basic Resource Management Commands

| Command                                     | Explanation                                                                                                                                       |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| `Connect-AzAccount`                         | Authenticates your Azure account and establishes a connection to your Azure subscription.                                                      |
| `Get-AzResourceGroup`                       | Lists all resource groups in your Azure subscription, helping you organize and manage your resources.                                          |
| `New-AzResourceGroup -Name <Name> -Location <Location>` | Creates a new resource group in a specified location, allowing you to organize resources logically.                                             |
| `Get-AzVM`                                 | Retrieves information about all virtual machines in your subscription, including their states and configurations.                               |
| `Start-AzVM -Name <VMName> -ResourceGroupName <ResourceGroup>` | Starts a specified virtual machine, allowing it to run and be accessible.                                                                        |
| `Stop-AzVM -Name <VMName> -ResourceGroupName <ResourceGroup>` | Stops (deallocates) a specified virtual machine, releasing its resources while preserving the configuration.                                     |
| `Remove-AzResourceGroup -Name <Name>`      | Deletes a specified resource group and all resources contained within it, which is useful for cleanup.                                          |
| `Get-AzStorageAccount`                      | Lists all storage accounts in your subscription, providing insight into your storage resources.                                                 |
| `New-AzStorageAccount -Name <Name> -ResourceGroupName <ResourceGroup> -Location <Location> -Sku <SkuType>` | Creates a new storage account with the specified parameters.                                                                                  |
| `Get-AzADUser`                             | Retrieves a list of Azure Active Directory users, useful for managing user access and roles within your Azure environment.                       |
