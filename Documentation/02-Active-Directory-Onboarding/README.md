# Active Directory Onboarding in SailPoint ISC

This documentation provides a hands-on walkthrough for onboarding Microsoft Active Directory into SailPoint Identity Security Cloud (ISC).

## What this covers

- Corporate Azure VNet and subnet design
- Network Security Group (NSG) configuration
- Active Directory Domain Controller deployment
- Active Directory Domain Services (AD DS) setup
- Organizational Units (OUs) and test users
- SailPoint service account creation
- SailPoint Virtual Appliance deployment
- Network connectivity between SailPoint VA and Active Directory
- LDAP / LDAPS connectivity
- SailPoint ISC source onboarding
- Account and entitlement aggregation
- Identity correlation
- Provisioning and lifecycle concepts
- Troubleshooting considerations

## Architecture

```text
                SailPoint Identity Security Cloud
                              |
                         HTTPS / 443
                              |
                     SailPoint VA
                     10.0.2.0/24
                              |
                    LDAP / LDAPS
                     389 / 636
                              |
                   Active Directory
                     10.0.1.0/24
