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
