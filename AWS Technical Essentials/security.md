Authentication
--------------

    If a user types in the correct email and password, the system assumes the user is allowed to enter and grants them access. This is the process of authentication. Authentication ensures that the user is who they say they are.

Authorization
--------------

    Authorization is the process of giving users permission to access AWS resources and services. Authorization determines whether a user can perform certain actions, such as read, edit, delete, or create resources. 

Best practices when working with the AWS root user
---------------------------------------------------

    * Choose a strong password for the root user
    * Never share your root user password or access keys with anyone
    * Disable or delete the access keys associated with the root user
    * Do not use the root user for administrative tasks or everyday tasks

(IAM) 
-----

    AWS Identity and Access Management 


IAM policies
------------

    To manage access and provide permissions to AWS services and resources, you create IAM policies and attach them to IAM users, groups, and roles. Whenever a user or role makes a request, AWS evaluates the policies associated with them