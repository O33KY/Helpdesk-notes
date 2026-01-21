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
  1.  Yellow exclamation  mark ->  missing faulty driver
  2.  Unknown device -> driver missing
  3.  Disabled device -> manual enable

 ## Task Manager

- To monitor system performance and running processes
  1. Processes - CPU, Memory, Disk, Network usage
  2. Apps impacting boot time
  3. Running background services
  4. Overall system condition
 
     ### Common actions
     
     - End unresponsive process
     - Identify  high CPU/RAM usage
     - Disable unnecessary apps
    
     **Always verify process before killing it**, **Startup tab when slow boot**

## Common commands

- ipconfig
- net user
- whoami
