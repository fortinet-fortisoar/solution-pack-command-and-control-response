## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

*Command and Control Response Solutions Pack* demonstrates the scenario and use cases around C&C response. The use-case deals with containment and investigation procedures once the end-user reports a Malware Alert.

### Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to Simulate and Reset scenarios.

Command and Control Response Solution Pack ships with the following simulation scenarios. 

**Command and Control Response**

The scenario generates a demo alert for the Alert Type **Malware**.

Navigate to generated alert and observe the following:

- Asset details like IP Address, Device UID are present
- Details such as Source Process, Process Name, File Hash are present to analyze the case

**Investigate Command & Control:**

Launch **Investigate Command & Control** playbook and observe how the playbook:

- Enriches alerts for command-and-control behavior by identifying the reputation of related artifacts such as source IP addresses and file hashes
- Identifies Geolocation of Source IP
- Investigates and terminates, using the CarbonBlack Response, anomalous processes running on the host that was the target of the attack
- Closes the alert after performing the tasks mentioned

## Prerequisite

Ensure that the following solution packs are deployed:

|**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules and Action playbooks|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Connectors

    |**Sr.No.**|**Connector**|
    | :- | :- |
    |1|CarbonBlack Response|
    |2|IPStack|
    |3|VirusTotal|

    **Warning:** After deployment, this Solution Pack will install or upgrade the stated connectors list.

2. Playbook Collection(s)

    - 02 - Use Case - Command & Control Response (1):

    |**Playbook Name**|**Description**|
    | :- | :- |
    |Investigate Command & Control|Enriches alerts for command-and-control behavior by identifying related artifacts' reputations, such as source IP addresses and file hashes. Terminates anomalous processes running on the host, which was target of the attack.|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
