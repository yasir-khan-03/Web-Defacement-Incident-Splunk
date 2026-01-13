# Web Defacement Incident Handling – Splunk

## Objective
To understand how SOC analysts investigate a website defacement incident using SIEM logs.

## Scenario
Wayne Enterprises reported that their website www.imreallynotbatman.com was defaced by attackers displaying an unauthorized message.

## Tool Used
- Splunk (SIEM)

## Dataset
- BOTS v1 Dataset

## Investigation Steps
1. Reviewed web traffic related to the affected domain
2. Analysed HTTP logs for suspicious activity
3. Identified repeated access attempts from suspicious IP addresses
4. Reviewed the timeline of events around the defacement

## Sample Splunk Searches
