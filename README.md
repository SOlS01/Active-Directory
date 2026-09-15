# Active-Directory

# Essential components of Active directory >> 

A windows domain is a group of users and computers under one administration.  the benefit of having it is centralised identity management and managing security policy. The repository called Active Directory where all the credentials are stored there. And the server that runs the Active Directory is known as Domain Controller. 

# Important groups in domain >>  

Domain Admin: high privilege, administrates all computers and resources in a domain 

Server Operators: they can administer Domain Controller but not any administrative group membership. 

Backup Operator: allowed to access to any file and perform backups of data on the PC 

Account Operators: users in this group can create or modify other accounts in the domain. 

 

# Organizational Units >> 
used to define set of users with similar policing requirements. But a user can only be a part of a single OU at a time. It is handy for applying the policies. 

# Security groups >> 
used to grant permission over resources, here a user can be a part of many groups which is needed to grant access to multiple resources. 

 

# Identifying machine accounts is easy, the machine account name is the computer’s name followed by a dollar sign. Soran-PC$ 

# Managing Users in AD >> 
to delete an OU we need to enable the Advanced Feature (view > Advanced Feature) because the credentials are protected with accidental deletion. > then go to that group properties and in the object unclick the protect object form accidental deletion. 

# Delegation >> 
allows us to grant users specific privileges to perform advanced task on OU without needing a domain admin to step in. Right click on the OU and typing the person’s name who we want to give privilege. This method mostly used for IT support. 
