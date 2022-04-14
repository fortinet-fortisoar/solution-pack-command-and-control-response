# Command and Control Response Solution Pack

## Overview

### Introduction

This article describes the Command and Control Response Solutions Pack. The solution pack demonstrates the scenarios and use cases around C&C response. The scenario demonstrates and generates a demo alert for the Alert Type 'Malware'. The use-case deals with containment and investigation procedures once the end-user reports a Malware Alert.

- Enriches alerts for command-and-control behaviour by identifying the reputation of related artefacts such as source IP addresses and file hashes.
- Find Geolocation of Source IP.
- Investigates any anomalous processes running on the host on which the attack has occurred are terminated using the CarbonBlack Response
- Close the Alert

### Usage

More information about usage/configuring of the Command and Control Response Solution Pack [here](https://github.com/fortinet-fortisoar/solution-pack-command-and-control-response/blob/develop/docs/solution-pack-guide.md).

## Version Information

- Solution Pack Version: 1.0.0
- FortiSOAR™ Version Tested on: 7.2.0
- Authored By: Fortinet
- Certified: No

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

    **Playbook Name**|**Description**
    | :- | :- |
    |Investigate Command & Control|Enriches alerts for command-and-control behaviour by identifying related artefacts' reputations such as source IP addresses and file hashes. Also, investigates any anomalous processes running on the host on which the attack has occurred are terminated.|

    **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.


