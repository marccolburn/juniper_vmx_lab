Juniper vMX Lab
======================
Create Juniper vMX lab in oVirt for testing various playbooks/scenerios.

This lab provides 10 vMXs that can be used to test various scenerios

Playbooks
---------
full_topology_lab.yml - will spin up networking and virtual machines within oVirt based on vars within vars/folder

Requirements
------------
* Ansible 2.9
* RAM ~ 60GB
* vCPUS ~ 50
* Templates for each of the VNF types

Caveats
-------
* ovirt_create_vms will not overwrite NIC profile if already assigned in template, (Recommend removing NICs from template and then assigning at creation)

Diagrams
--------
## Juniper vMX Lab Logical with Addressing
![Logical Overview](/images/vmx_lab_logical_overview.svg)
