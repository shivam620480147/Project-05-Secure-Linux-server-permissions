# Project 5: Secure Linux Server Permissions

## Objective
Implement user-based access restrictions on an Ubuntu Linux server using Linux users, groups, ownership, and file permissions.

## Environment
- OS: Ubuntu 24.04.3 LTS
- Users: project5_admin, project5_user
- Groups: project5_admins, project5_users

## Implementation
1. Created two Linux groups and two test users.
2. Added the admin user to project5_admins.
3. Kept the normal user outside the admin group.
4. Created /opt/project5/secure.
5. Assigned ownership to root:project5_admins.
6. Set directory permissions to 770.
7. Created secret.txt and set permissions to 660.

## Test Results
- Admin user successfully read the confidential file.
- Normal user received Permission denied when attempting to read it.
- Normal user received Permission denied when attempting to create a file.
- Directory permissions were verified.

## Conclusion
Linux user and group management, ownership, and file permissions were used to restrict access to confidential files. The tests confirmed that authorized users could access the protected directory while unauthorized users were denied.
