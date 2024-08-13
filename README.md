# Linux File Ownership and Permissions

## Scenario
In this project i am  a security professional at a large organization, working with the research team to ensure users have appropriate permissions. My task is to examine existing permissions on the file system, determine if they match the required authorization, and modify them if necessary. This task is part of my Google Cybersecurity Certification, focusing on using Linux commands to manage file permissions.

## Step-by-Step Instructions

1. **Examine Existing Permissions**
   - Use the `ls -l` command to list the directory contents with detailed information about file permissions, owners, and groups.
   - Example command:
     ```bash
     ls -l /projects
     ```

2. **Determine Authorization**
   - Compare the existing permissions with the required permissions for the research team.
   - Identify any discrepancies where permissions do not match the required authorization.

3. **Modify Permissions**
   - Use the `chmod` command to modify file permissions as needed.
   - Example command to add execute permission for the group:
     ```bash
     chmod g+x /projects/drafts
     ```

4. **Verify Changes**
   - Re-run the `ls -l` command to verify that the permissions have been updated correctly.
   - Ensure that unauthorized access has been removed and appropriate users have the necessary permissions.

## Initial Permissions
The initial permissions for the files and directories in the `/projects` directory are as follows:

```plaintext
total 20
drwxr-xr-x 2 researcher2 research_team 4096 Aug 12 12:47 drafts
-rw-rw-r-- 1 researcher2 research_team   46 Aug 12 12:47 project_k.txt
-rw-rw-r-- 1 researcher2 research_team   46 Aug 12 12:47 project_l.txt
-rw-rw-r-- 1 researcher2 research_team   46 Aug 12 12:47 project_m.txt
