# OneDrive Cloud Forensics  

## Locations of Interest:  
%USERPROFILE%\OneDrive
NTUSER.DAT\Software\Microsoft\OneDrive\Accounts  
- Personal  
- Business
NTUSER.DAT\Software\Microsoft\OneDrive\Accounts\Business1\Tenants  

Provides:  
Personal: UserEmail, UserFolder, cid  
Business: UserEmail, UserFolder, cid, SPOResourceID  

### Tools of interest:  
OneDrive Explorer GUI  
- Options\ Preference - Autosave to CSV.  Autosave Path.  
- Load <UserCid>.dat
-  Example file path: E:\C\Users\username\AppData\Local\Microsoft\OneDrive\settings\Personal\e4345543.dat
-  E:\C\username\NTUSER.DAT
-  E:\C\$Recycle.Bin\S-1-5-21-XXX-XXX-1002
-  
