# Copilot for Security Custom Plugin - API - Get Shodan Product Distribution

#### Copilot for Security Plugin to gather Shodan Product version distribution using Shodan's API's

### Pre-requisites

* [Copilot for Security Enabled](https://learn.microsoft.com/en-us/security-copilot/get-started-security-copilot#onboarding-to-microsoft-security-copilot)
* [Access to upload custom plugins](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#managing-custom-plugins)
* [API Key](https://developer.shodan.io/api/requirements) from Shodan.io

### Instructions
#### Upload the Custom Plugin

1. Obtain the file [API-GetShodanProduct.yaml](https://github.com/SCStelz/CopilotForSecurity/blob/main/CustomPlugIns/API-GetShodanIP/API-GetShodanIP.yaml) from this directory.
2. [Upload the custom plugin](https://learn.microsoft.com/en-us/security-copilot/manage-plugins?tabs=securitycopilotplugin#add-custom-plugins) and verify it's activated.
3. After plugin upload put in your [Shodan API Key](https://learn.microsoft.com/en-us/security-copilot/plugin_api#configure-authentication-1).

![CopilotForSecurity](https://learn.microsoft.com/en-us/security-copilot/media/add-plugin-button.png)

### Plugin Utilization

Here's some sample queries you can utilize to trigger this plugin

* Can you lookup a version distribution of Plex Media Server from Shodan?
<br>
<img src="https://github.com/SCStelz/CopilotForSecurity/blob/main/Images/shodan-product-masked.png"/>

You can start an investigation with the [API-GetShodanIP Plugin](https://github.com/SCStelz/CopilotForSecurity/tree/main/CustomPlugIns/API-GetShodanIP) to get running services on a particular IP address, then follow up with this plugin to validate product distribution.
<br>
