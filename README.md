# ansible-role-openshift_cluster_login

Ansible role for logging into an OpenShift cluster using `oc` tools.

## Role Parameters

You must set either ocp_token, or both ocp_user and ocp_password.

| parameter                     | required  | default       | choices         | comments 
| ------------------------------|:---------:|:-------------:| --------------- | :-------- 
| ocp\_url                      | yes       |               |                 | URL to OCP cluster to log into
| ocp\_user                     | sometimes |               |                 | User to log in as. Required if ocp_token is not set.
| ocp\_password                 | sometimes |               |                 | User password. Required if ocp_token is not set.
| ocp\_token                    | sometimes |               |                 | Authentication token to use for login. Required if ocp_passord and ocp_url are not set.
| ocp\_login\_skip\_tls\_verify | no        | false         | true, false     | Skip TLS verify
