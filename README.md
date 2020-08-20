# openshift-haproxy
This is a small ansible role to modify the HAProxy config on a designated `[lb]` machine used in OpenShift 3.

It should be run against the inventory file you are using for your OCPlatform 3 install.

# Assumptions:
  * You have a section in your inventory designating `[masters]` and `[infra]`
  * It is run against the node in the `[lb]`

Parameters can be modified in the `roles/templates/haproxy.cfg.j2` file if the values need to be changed. 
