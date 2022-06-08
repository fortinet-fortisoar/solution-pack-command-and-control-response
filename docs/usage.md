| [Home](https://github.com/fortinet-fortisoar/solution-pack-command-and-control-response/blob/develop/README.md) | 
|--------------------------------------------| 

# Usage 
 
Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/usage.md) to understand how to simulate and reset scenarios. 
 
To understand the process FortiSOAR follows to respond to alerts relating to Command and Control behavior, we have included a scenario &mdash; **Command and Control Response** with this solution pack. Refer to the section *Command and Control Response* to understand how this solution pack's automation addresses your needs.

## Command and Control Response

This scenario generates an example alert of Type *Malware* in FortiSOAR's **Alerts** module.

Navigate to demo alert and note the following:

- The demo alert created is an example of a default data ingestion using the **Data Ingestion** feature
- The alert is of type *Malware*
- The reported alert contains the following among other related sources data:
    - Asset details
        - IP Address
        - Device UID
    - Source IP address
    - Source Process
    - Process Name
    - Destination IP address
    - File hash
- The playbook **Investigate Command & Control** appears as one of the options under **Execute** drop-down once you select the demo alert

### Investigate Command & Control

This playbook performs the following automated tasks:

- Enriches alerts for command-and-control behavior by identifying the reputation of related artifacts such as source IP addresses and file hashes
- Identifies Geolocation of Source IP
- Investigates and terminates, using the CarbonBlack Response, anomalous processes running on the targetted host
- Closes the alert after performing the above tasks