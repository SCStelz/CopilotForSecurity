# Get Virus Total IP Information

#### Copilot for Security Plugin to gather reputation information for an IP Address using Virus Total API's

### Pre-requisites

* [Copilot for Security Enabled](https://learn.microsoft.com/en-us/security-copilot/get-started-security-copilot#onboarding-to-microsoft-security-copilot)
* [Access to upload custom plugins](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#managing-custom-plugins)
* [API Key](https://docs.virustotal.com/docs/please-give-me-an-api-key) from VirusTotal.com

### Instructions
#### Upload the Custom Plugin

1. Obtain the file [API-GetAbuseIPDBIP.yaml](https://github.com/SCStelz/CopilotForSecurity/blob/main/CustomPlugIns/API-GetVirusTotalIP/API-GetVirusTotalIP.yaml) from this directory.
2. [Upload the custom plugin](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#add-custom-plugins) and verify it's activated.
3. After plugin upload put in your [Virus Total API Key](https://learn.microsoft.com/en-us/security-copilot/plugin_api#configure-authentication-1).

![CopilotForSecurity](https://learn.microsoft.com/en-us/security-copilot/media/add-plugin-button.png)

### Plugin Utilization

Here's some sample queries you can utilize to trigger this plugin

* Can you summarize the Virus Total information for the IP 185.220.101.140?
* Can you output a table I can export of the reputation information from all the engines from Virus Total for the IP 185.220.101.140?
* Which engines detected the IP 185.220.101.140 as malicious from Virus Total?
<br>
<img src="https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/virustotal.png"/>

