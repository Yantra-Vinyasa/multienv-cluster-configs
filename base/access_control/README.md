# WIP..... 

# Access Control
This directory holds the base configuration for **access control** components.

## Components
* ldap
* group-sync

## Configuration 
Configure OpenShift to use LDAP for user authentication

To restrict access to the OCP based on users managed on an LDAP server, an Identity Provider LDAP must be configured. 

The following information must be available to configure LDAP-based authentication:

* Username (called Bind DN) and password (called Bind Password) of a user having access to the LDAP tree (if anonymous access is disabled)
* Protocol, hostname and port of the LDAP server
* LDAP Server Certificate Authority Chain (if LDAP connection is secure)
* Base DN location for which users will be searched for
* Additional filtering logic, such as the scope of the user's query and a filter (optional)
