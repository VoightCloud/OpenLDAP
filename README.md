# OpenLDAP
This will install an OpenLDAP instance in your kubernetes cluster.

https://github.com/helm/charts/blob/master/stable/openldap/values.yaml

## Note:
You must have a site-cert and a site-ca secret installed in the same namespace
as your OpenLDAP server before starting. If you don't have them, you will
need to disable TLS.

### Usage
#### Installation

```shell script
ansible-playbook --vault-password-file=~/vaultpwd ./playbook.yaml
```
#### Removal
```shell script
ansible-playbook ./reset.yaml
```
