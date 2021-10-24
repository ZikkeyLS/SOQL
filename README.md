# *SOQL*
SOCL - string oriented query language (partially based on SQL standarts)

### TIL – Table Interaction Language
* **CREATE** - create table;
* **EDIT** - edit table;
* **REMOVE** - remove table;
### ERL – Element Redact Language
* **GET** – get element;
* **INSERT** – add element;
* **CHANGE** – change element;
* **DELETE** – remove element;

## Description
### TIL
* **CREATE** 

  **Arguments:**
  
    CREATE [*TABLE_NAME*] [*arguments*(unrequired)]
  
  **Examples:**
  
    ```[*TABLE_NAME*] = TEST
  
    [*arguments*] = user_token(U), user_name(U, Min(4), Max(16)), user_password(Min(6), Max(20))
  
    CREATE [*TABLE_NAME*] [*arguments*]
    ```
    
* **EDIT**

  **Arguments:**
  
    EDIT STRUCTURE [*TABLE_NAME*] [*arguments*]
  
    EDIT NAME [*TABLE_NAME*] [*NEW_TABLE_NAME*]
  
  **Examples:**
    ```
    [*arguments*] = user_token(U), user_name(U, Min(4), Max(16)), user_password(Min(6), Max(20), user_status))
    
    EDIT STRUCTURE TEST [*arguments*]
    
    -------------------------------------------
    
    EDIT NAME TEST TEST1
    ```
    
* **DELETE**

  **Arguments:**
  
    DELETE [*TABLE_NAME*]  
    
  **Examples:**
    ```
    DELETE TEST
    ```
