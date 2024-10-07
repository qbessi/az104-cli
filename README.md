# AZ104 PowerSHell Command Dump
A PowerShell command dump used for the AZ-104 exam.

<details>
<summary>
How do I connect to Azure from PowerShell?
</summary>
    Connect-AzAccount
</details>


<details>
<summary>
What are the Azure PowerShell and CLI commands to create a security group called IT Admins? Provide the official command reference page.
</summary>
New-AzADGroup -DisplayName "IT Admins" -MailNickname $false
</details>


<details>
<summary>
How do you delete a Resource Group?
</summary>
Remove-AzResourceGroup -Name resourceGroupName
</details>


| Command                                      | Explanation                                                                                                                                       |
|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| `Get-AzSubscription`                         | Retrieves a list of all subscriptions associated with your Azure account. This command provides details such as the subscription ID, name, and state. |
| `Select-AzSubscription -SubscriptionId <ID>`| Sets the specified subscription as the current active subscription for the session, allowing subsequent commands to operate within that context.   |
| `Get-AzContext`                             | Displays the current Azure context, including the active subscription and tenant details. Useful for confirming which subscription you're working in.  |
| `Get-AzAccount`                             | Lists all accounts associated with your Azure environment, including subscription information. This command helps verify which subscriptions you can access. |
| `Get-AzRoleAssignment -Scope <Scope>`      | Retrieves role assignments at the specified scope (such as a subscription). This helps you understand who has access to resources in that subscription. |
