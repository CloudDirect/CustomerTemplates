# Customer Templates

This is the set of master templates and parameter files.

All of the master templates reflect a high level design architecture.  They make use of Cloud Direct's set of Azure Resource Manager template modules, which are centralised and non-customisable.

The master templates may be customised.  The customer's configuration requirements feed into the parameter files, e.g. customer tags, naming for vNets and subnets, address prefixes and subnetting, etc.

This read only repo is used as a template source, and should be copied into the customer's subscription using DevOps Projects so that the customer has its own Git repository for versioning the Infrastructure as Code.

Before deploying using these file it is assumed that the user and groups have been predefined and policies have been applied.