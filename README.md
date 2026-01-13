# Web Defacement Incident Handling – Splunk

## Objective
To understand how SOC analysts investigate a website defacement incident using SIEM logs.

## Scenario
Wayne Enterprises reported that their website **www.imreallynotbatman.com** was defaced by attackers displaying an unauthorized message.

## Tool Used
- Splunk (SIEM)

## Dataset
- BOTS v1 Dataset

## Investigation Steps
- Reviewed web traffic related to the affected domain
- Analysed HTTP logs for suspicious activity
- Identified repeated access attempts from suspicious IP addresses
- Reviewed the timeline of events around the defacement

## Sample Splunk Searches
```spl
index=botsv1 imreallynotbatman
index=botsv1 sourcetype=stream:http
index=botsv1 | stats count by src_ip
## Findings
- Suspicious HTTP traffic was observed targeting the affected domain
- Repeated requests were identified from the same source IP address
- The activity indicates possible unauthorized access leading to website defacement
## Outcome
This project helped me understand how SOC analysts investigate website defacement incidents using SIEM tools like Splunk by analysing logs and identifying suspicious activity.


