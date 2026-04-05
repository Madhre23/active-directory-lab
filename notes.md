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

## Managing Computers in AD
- Added computers to the domain for centralized management

## Group Policy (GPO)
- Used to enforce rules across the network
- Example: password policies, restrictions

## Authentication
- Active Directory uses Kerberos authentication

## Trees, Forests, Trusts
- Tree: Multiple domains grouped together
- Forest: Collection of domain trees
- Trust: Allows communication between domains

## Key Takeaways
- Centralized management is more efficient
- Group-based permissions simplify access control

---

## Personal Notes
- I was confused at first about OUs vs Groups but realized OUs are for organization, not permissions  
- Group Policy seems powerful but can affect the whole domain if misconfigured  
- Seeing how everything is centralized helped me understand how companies manage large networks  
