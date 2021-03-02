# WatchGuard Firewall Cluster ArcSight FlexConnector

## Summary
Parse events from a WatchGuard Firebox Firewall (Clustered)
## References
* https://www.watchguard.com/help/docs/fireware/12/en-US/log_catalog/Log-Catalog_v12_6.pdf
## Scope
Cluster and Firewall logs
## Technical Details
* Vendor: WatchGuard
* Product: Firebox
* Version Tested: Clustered M270 Fireware Version 12.5.2 & Clustered XTM330 Fireware 12.1.3 
* Developed on SmartConnector version: 8.0

## Log Source Configuration
configure Syslog to send to the ArcSight SmartConnector destination.

## Constraints

## SmartConnector Installation:
Install the ArcSight Syslog SmartConnector as per the vendor or your organisations guidance

## FlexConnector Configuration:
Copy the fcp, flexagent and acp folders and the contents to the below folder on the SmartConnector
* <CONNECTOR_HOME>/current/user/agent/
Restart the SmartConnector

## Testing:
* Review the logs for any error
* Create a filter / channel based on: deviceVendor="WatchGuard" AND deviceProduct="firebox"

## To Do
Additional parsing of modules other than Firewall
