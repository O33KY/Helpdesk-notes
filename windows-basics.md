# Windows Basics

## User accounts

- Local users vs domain users - local exists only on one machine, domain users managed by **Active Directory** (central management of users, computers & permissions)
- Administrator vs standard user 
- **RUN** -->  `lusrmgr.msc`  for managing the groups & local users
- Local file permissions

## Event Viewer & logs

- For troubleshooting system & app issues
- **SYSTEM**,  **APPS**, **SECURITY**

## Device Manager

- For hardware troubleshooting & driver management
- Yellow exclamation  mark ->  missing faulty driver
-  Unknown device -> driver missing
-    Disabled device -> manual enable

 ## Task Manager

- To monitor system performance and running processes
- Processes - CPU, Memory, Disk, Network usage
- Apps impacting boot time
- Running background services
- Overall system condition
 
     ### Common actions
     
     - End unresponsive process
     - Identify  high CPU/RAM usage
     - Disable unnecessary apps
    
     **Always verify process before killing it**, **Startup tab when slow boot**

     ### Services
 
     -  **RUN** -> `services.msc`
     - Programs running in the background
     - Crucial for system and network running properly (no Win Update - no Update, no DHCP((assigns IP address)) Client - no IP, no Print Spooler - no printing etc.)

     **Don't disable services w/o understanding what it does**

  ## Windows Registry

  - Database for configuration settings for OS and installed apps
    
          HIVES: 
    - HKLM (HKEY_LOCAL_MACHINE) -> system settings
    - HKCU (HKEY_CURENT_USER) -> current user settings
    - HKCR (HKEY_CLASSES_ROOT) -> file associations (fundamental, highest-level class or element from which others inherit or are defined, providing essential structure or settings)
    - HKU -> all users
   
      
    - Keys & values
      
 ~~~
HKLM Hive
 └── Software  Key
     └── Microsoft Key
~~~

  - Used for apps troubleshooting, user settings reset, malware checks
  
  **Always backup before changes**
  **Malware often -> HKCU\Software\Microsoft\Windows\CurrentVersion\Run**


## Common commands

- ipconfig
- net user
- whoami
