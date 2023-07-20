# Group Synchronization
This component is for maintaining and working with the group synchronization for the OpenShift environment.
It will install the group-sync operator and a _group_sync_ object that will pull groups from Active Directory to the clusters.

The LDAP identity provider is handled through a _secret_ in the openshift-config _project_ and cluster wide _OAuth_ resource. [LDAP in OCP](https://docs.openshift.com/container-platform/latest/authentication/identity_providers/configuring-ldap-identity-provider.html)
 
## Configuration
Add groups to OpenShift by adding an entry for them in the whitelist in the _group-sync.yaml_ object.

```yaml
      whitelist:

```

## Useful commands


```sh
oc get groups
N
```

## Troubleshooting
[OpenShift Documentation on LDAP syncing](https://docs.openshift.com/container-platform/latest/authentication/ldap-syncing.html)
