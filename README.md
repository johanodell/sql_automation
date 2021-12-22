# sql_automation
This repo contains playbooks for automating the provisioning of a RHEL virtual machine running Microsoft SQL server in a vSphere cluster.
It is quick and dirty for a demo i am working on 
The state of the repo is work in progress. The process is utilising some services which require subscription entitlements. 

See workflow below

![Alt text](images/sql_automation.png?raw=true "high level process")

Work in progress: 
- add monitoring of sql metrics via performance co-pilot and visualization in grafana 
- deploy multiple servers in the same process 