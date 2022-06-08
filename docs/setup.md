| [Home](https://github.com/fortinet-fortisoar/solution-pack-command-and-control-response/blob/develop/README.md) | 
|--------------------------------------------| 

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search for and select **Command and Control Response**.
3. Click the **Command and Control Response** solution pack card.
4. Click the **Install** button on the bottom to begin installation.

## Prerequisite

The **Command and Control Response** solution pack depends on the following solution packs. 

| Solution Pack Name | Purpose   | 
| :--------------------- | :--------------------------------------- | 
| SOAR Framework | Required for Incident Response modules   | 
| SOC Simulator  | Required for Scenario Module and SOC Simulator connector | 

# Configuration 
For optimal performance of **Command and Control Response** solution pack, you can install and configure:

- Threat intelligence connectors to enrich context of a given indicator 
    - To configure and use the VirusTotal connector as a source of threat intelligence, refer to [Configuring Virus Total](https://docs.fortinet.com/document/fortisoar/2.1.0/virustotal/166/virustotal-v2-1-0#Configuration_parameters) 
- An Endpoint Detection and Response(EDR) solution
    - To configure and use the CarbonBlack Response connector as an EDR solution, refer to [Configuring CarbonBlack Response](https://docs.fortinet.com/document/fortisoar/2.0.1/carbonblack-response/1/carbonblack-response-v2-0-1#Configuration_parameters) 