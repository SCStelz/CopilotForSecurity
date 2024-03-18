# Sentinel KQL OfficeActivity Logs

#### Copilot for Security Plugin to run a Dynamic KQL Query for a particluar user, IP Address and time and date range against the OfficeActivity logs in a Microsoft Sentinel workspace.

### Pre-requisites

* [Copilot for Security Enabled](https://learn.microsoft.com/en-us/security-copilot/get-started-security-copilot#onboarding-to-microsoft-security-copilot)
* [Access to upload custom plugins](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#managing-custom-plugins)
* [Microsoft Sentinel Workspace](https://learn.microsoft.com/en-us/azure/sentinel/quickstart-onboard) created.
* Microsoft Sentinel [Microsoft 365 Data Connector]([Microsoft Sentinel Workspace](https://learn.microsoft.com/en-us/azure/sentinel/quickstart-onboard) created.) enabled.
* Parameters for KQL Plugin - Microsoft Sentinel Workspace Name, Subscription ID, Resource Group Name and Entra Tenant ID

### Instructions
#### Upload the Custom Plugin

1. Obtain the file [API-GetShodanIP.yaml](https://github.com/SCStelz/CopilotForSecurity/blob/main/CustomPlugIns/API-GetShodanIP/API-GetShodanIP.yaml) from this directory.
2. Modify the yaml file to specify your specific Entra TentantId, SubscriptionId, ResourceGroupName and WorkspaceName for your Sentinel instance. ie.
![KQLConnection](https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/kql-connection.png)
4. [Upload the custom plugin](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#add-custom-plugins) and verify it's activated.

![CopilotForSecurity](https://learn.microsoft.com/en-us/security-copilot/media/add-plugin-button.png)

### Plugin Utilization

Here's some sample queries you can utilize to trigger this plugin

* Can you describe the Office 365 Activity logs in detail over a few paragraphs for the IP x.x.x.x between Dec 3rd and Dec 4th?

![O365Logs](https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/O365logs-Masked.png)


