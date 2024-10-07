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
