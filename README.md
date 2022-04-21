# Command and Control Response Solution Pack

## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

*Command and Control Response Solutions Pack* demonstrates the scenario and use cases around C&C response. The use-case deals with containment and investigation procedures once the end-user reports a Malware Alert.


### Usage

This Solution Pack ships with following simulation scenarios. [Refer](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to Simulate Scenario documentation to undersand how to Simulate and Reset Scenario.

#### 1. Scenario: Command and Control Response

The scenario generates a demo alert for the Alert Type 'Malware'.

Goto generated alert and observe the following:

- Asset details like IP Addesss, Device UID is presented
- Also details such as Source Process, Process Name, File Hash presented to analying the case

**Investigate Command & Control:**

Launch "Investigate Command & Control" playbook and observe various investigation activities such as

- Enriches alerts for command-and-control behaviour by identifying the reputation of related artefacts such as source IP addresses and file hashes.
- Find Geolocation of Source IP.
- Investigates any anomalous processes running on the host on which the attack has occurred are terminated using the CarbonBlack Response
- Close the Alert

## Prerequisite

Ensure that the below solution packs are deployed:

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
    Following is a list of playbooks in this solution pack.

    |**Playbook Name**|**Description**|
    | :- | :- |
    |Investigate Command & Control|Enriches alerts for command-and-control behaviour by identifying related artefacts' reputations such as source IP addresses and file hashes. Also, investigates any anomalous processes running on the host on which the attack has occurred are terminated.|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
