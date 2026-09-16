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

Always segregate the devices according to their use try to have different containers to separate them. 

# Group policies >> 
to configure a group policy we can use the group policy management on windows, first we create a group policy object then link it to the OU where we want to apply the policy by drag and drop. 

# There are two methods/protocols for network authentication: 

# Kerberos >> 
it is ticket as proof of a previous authentication, key distribution centre KDC is in charge of creating Kerberos tickets on the network. The ticket granting ticket TGT allow the user to request additional ticket to access to service,  

and  

# NetNTLM >>
with this protocol the user’s password or hash password never transmitted through the network for security. 

# Tree >> when we got other branches in our company, but we don’t want the UK to be independent from US so we can create a tree. (one windows domain that share the same namespace) 

# Forest >> when the union of several trees with different namespaces into the same network is known as a forest. 

# Trust >> when the tree and forest in some points needs to share their file this domain is created under trust relationship. There is one way or two-way trust relationship.
