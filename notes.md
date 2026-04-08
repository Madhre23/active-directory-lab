# Active Directory Lab Notes

## What is Active Directory?
Active Directory (AD) is a directory service used to manage users, computers, and permissions in a network. It allows centralized control instead of managing each computer individually.

## Windows Domains
A domain is a network where all users and computers are managed centrally through a Domain Controller.

## Domain Controller (DC)
- Authenticates users when they log in
- Stores user and computer information
- Enforces security policies

## Users and Groups
- Users: Individual accounts for each person
- Groups: Used to assign permissions to multiple users at once

## Organizational Units (OUs)
- Used to organize users and computers
- Helps apply policies to specific parts of the organization

## Managing Users in AD
- Created user accounts
- Assigned users to groups
- Delegation: allows you to grant users specific privileges to perform advanced tasks on OUs without needing a Domain Administrator to step in.

## Managing Computers in AD
- Added computers to the domain for centralized management
- segregating devices according to their use
- Workstations, servers, domain controllers (main devices)
- Domain controllers most sensitive devices (security wise)
  

## Group Policy (GPO)
- Used to enforce rules across the network
- Example: password policies, restrictions
- simply a collection of settings that can be applied to OUs. GPOs can contain policies aimed at either users or computers, allowing you to set a baseline on specific machines and identities.
- GPOs are distributed to the network via a network share called SYSVOL, which is stored in the DC

## Authentication
- Active Directory uses Kerberos authentication
- Users who log into a service using Kerberos will be assigned tickets.
- Think of tickets as proof of a previous authentication.
- Users with tickets can present them to a service to demonstrate they have already authenticated into the network before and are therefore enabled to use it.

## Trees, Forests, Trusts
- Tree: Multiple domains grouped together
- Forest: Collection of domain trees
- Trust: Allows communication between domains
-  If you have two domains that share the same namespace, those domains can be joined into a Tree.
-  Two-way trust relationships can also be made to allow both domains to mutually authorise users from the other.
-   joining several domains under a tree or a forest will form a two-way trust relationship.

## Key Takeaways
- Centralized management is more efficient
- Group-based permissions simplify access control

---

## Personal Notes
- I was confused at first about OUs vs Groups but realized OUs are for organization, not permissions  
- Group Policy seems powerful but can affect the whole domain if misconfigured  
- Seeing how everything is centralized helped me understand how companies manage large networks
  
