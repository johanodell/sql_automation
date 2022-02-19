# sql_automation
This repo contains playbooks for automating the provisioning of a RHEL virtual machine running Microsoft SQL server in a vSphere cluster.
It is quick and dirty for a demo i am working on. The state of the repo is work in progress. The process is utilising some services which require subscription entitlements. To be able to use these playbooks you will need subscriptions for RHEL (OS, Red Hat Insights, RHEL-system-roles) as well as Ansible Automation Platform. 

See workflow below

![Alt text](images/sql_automation_workflow.png?raw=true "high level process")


My environment looks like below

![Alt text](images/environment.png?raw=true "environment")

First, if you already have an Ansible Automation Controller up and running you can add this repo by using the playbook ansible_controller_create_mssql_project.yml

Do the following steps to setup the central monitoring server with pcp and grafana. 
- If needed deploy a rhel-vm using an existing template or you can use the playbook deploy_rhel_on_vsphere.yml

- Run the playbook called setup_central_monitoringsystem.yml against the new VM. 
