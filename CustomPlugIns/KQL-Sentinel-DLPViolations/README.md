# Sentinel KQL DLP Audit Logs

#### Copilot for Security Plugin to run a Dynamic KQL Query for a particluar user, IP Address and time and date range against the Unified audit logs table *O365_CL* in a Microsoft Sentinel workspace.

### Pre-requisites

* [Copilot for Security Enabled](https://learn.microsoft.com/en-us/security-copilot/get-started-security-copilot#onboarding-to-microsoft-security-copilot)
* [Access to upload custom plugins](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#managing-custom-plugins)
* [Microsoft Sentinel Workspace](https://learn.microsoft.com/en-us/azure/sentinel/quickstart-onboard) created.
* Microsoft Sentinel [Unified Audit Logs Connector](https://github.com/sreedharande/IngestOffice365AuditLogs) enabled, this pull's in additional DLP.All events into a custom O365_CL table.
* Parameters for KQL Plugin - Microsoft Sentinel Workspace Name, Subscription ID, Resource Group Name and Entra Tenant ID

### Instructions
#### Upload the Custom Plugin

1. Obtain the file [KQL-Sentinel-DLPViolations.yaml](https://github.com/SCStelz/CopilotForSecurity/blob/main/CustomPlugIns/KQL-Sentinel-DLPViolations/KQL-Sentinel-DLPViolations.yaml) from this directory.
2. Modify the yaml file to specify your specific Entra TentantId, SubscriptionId, ResourceGroupName and WorkspaceName for your Sentinel instance.

![KQLConnection](https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/kql-connection.png)

4. [Upload the custom plugin](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#add-custom-plugins) and verify it's activated.

![CopilotForSecurity](https://learn.microsoft.com/en-us/security-copilot/media/add-plugin-button.png)

### Plugin Utilization

Here's some sample queries you can utilize to trigger this plugin

* Can you describe in detail over a few paragraphs a timeline of events coming from the recent DLP violations for the user user@contoso.com from the past 90 days? Be sure to include all relevant DLP violation details
* Can you provide a list of sensitive files that have been uploaded to the cloud from the recent DLP violations for user@contoso.com in the past 90 days?

![CopilotForSecurity](https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/dlp-masked.png)


