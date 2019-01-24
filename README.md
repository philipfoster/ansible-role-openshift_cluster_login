# ansible-role-openshift_cluster_login

Ansible role for logging into an OpenShift cluster using `oc` tools.

## Role Parameters

| parameter                     | required | default       | choices         | comments 
| ------------------------------|:--------:|:-------------:| --------------- | :-------- 
| ocp\_url                      | yes      |               |                 | URL to OCP cluster to log into
| ocp\_user                     | yes      |               |                 | User to log in as
| ocp\_password                 | yes      |               |                 | User password
| ocp\_login\_skip\_tls\_verify | no       | false         | true, false     | Skip TLS verify
