---
date: 2024-03-23 
tags: 
      - Database
---
# Data Control Language
## GRANT Command
- Use a command that gives privilege access to data.
  - System Privilege
  - Object Privilege
    - Access to User
### Object Privilege
- Create Privilege 
  - Use Grant Command 
  ```sql
  GRANT SELECT ON TABLE table_name TO User_Name
  ```
  ```sql
  GRANT ALL ON TABLE table_name TO User_Name,User_Name
  ```
    - User can share privilege with other user
      ```sql
      GRANT SELECT ON TABLE table_name TO User_Name WITH GRANT OPTION
      ```
- Remove Privilege
  - Use Revoke Command
    ```sql
    REVOKE UPDATE ON TABLE table_name FROM User_Name
    ```
    ```sql
    REVOKE ALL ON TABLE table_name FROM User_Name,User_Name
    ```