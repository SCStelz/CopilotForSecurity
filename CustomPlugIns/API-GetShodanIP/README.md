# Get Shodan IP Information

#### Copilot for Security Plugin to gather reputation and running services for an IP Address using Shodan's API's

### Pre-requisites

* [Copilot for Security Enabled](https://learn.microsoft.com/en-us/security-copilot/get-started-security-copilot#onboarding-to-microsoft-security-copilot)
* [Access to upload custom plugins](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#managing-custom-plugins)
* [API Key](https://developer.shodan.io/api/requirements) from Shodan.io

### Instructions
#### Upload the Custom Plugin

1. Obtain the file [API-GetAbuseIPDBIP.yaml](https://github.com/SCStelz/CopilotForSecurity/blob/main/CustomPlugIns/API-GetShodanIP/API-GetShodanIP.yaml) from this directory.
2. [Upload the custom plugin](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#add-custom-plugins) and verify it's activated.
3. After plugin upload put in your [Shodan API Key](https://learn.microsoft.com/en-us/security-copilot/plugin_api#configure-authentication-1).

![CopilotForSecurity](https://learn.microsoft.com/en-us/security-copilot/media/add-plugin-button.png)

### Plugin Utilization

Here's some sample queries you can utilize to trigger this plugin

* Can you summarize the Shodan information for the IP 185.220.101.140?
<br>
<img src="https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/Shodan-ip.png"/>
<br>
<img src="https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/shodan-ip-2-masked.png"/>

You can follow up a question with the [API-GetShodan-Product Plugin](https://github.com/SCStelz/CopilotForSecurity/tree/main/CustomPlugIns/API-GetShodanProduct) to validate worldwide version distribution of the particluar product.
*Based on the product on the open port, can you get a version distribution form Shodan? Is this product the latest?
<img src="https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/shodan-product-masked.png"/>

