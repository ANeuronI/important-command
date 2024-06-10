# Important-Command
some important command which is very much used

---

1. # Virtual env in windows and Linux
   
     1. ### Creating the virtual environment same in both linux and windows 
     
         ``` virtualenv myenv ```
   
     2. ### Activating virtual env

           #### Activating virtual env in Windows :
     
             ``` myenv\Scripts\activate.bat```

           #### Activating virtual env in Linux :
     
            ``` source myenv/bin/activate ```
            
    3. ### De - activating virtual env
    
            ``` deactivate```
---

2.   #### some time activating the environment in windows is blocked by terminal due to sequrity access
      
       1. ### Check Current Execution Policy:
          
           ``` Get-ExecutionPolicy ```
          
       2. ### Set Execution Policy:
  
           #### RemoteSigned :
          
             Requires that all scripts and configuration files downloaded from the Internet be signed by a trusted publisher.

             ```  Set-ExecutionPolicy RemoteSigned ```
          
           #### Unrestricted :
          
            Allows all scripts and configuration files to run. If you run an unsigned script that was downloaded from the Internet, you will be prompted for permission before it runs.

          ```  Set-ExecutionPolicy Unrestricted ```
          
       4.   #### those policy can be applied for current users which was signed in or can be used by current session :

             #### current user :

             ``` Set-ExecutionPolicy RemoteSigned -Scope CurrentUser  ```

            ### current session :

            ``` Set-ExecutionPolicy RemoteSigned -Scope Process ```

       5.   #### Revert Execution Policy:

             ``` Set-ExecutionPolicy Restricted ```
            
---
