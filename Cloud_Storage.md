# OneDrive and Google

## OneDrive

### Locations of Interest:  
%USERPROFILE%\OneDrive
NTUSER.DAT\Software\Microsoft\OneDrive\Accounts  
- Personal  
- Business
NTUSER.DAT\Software\Microsoft\OneDrive\Accounts\Business1\Tenants  

Provides:  
Personal: UserEmail, UserFolder, cid  
Business: UserEmail, UserFolder, cid, SPOResourceID  

#### Tools of interest:  
OneDrive Explorer GUI  
- Options\ Preference - Autosave to CSV.  Autosave Path.  
- Load <UserCid>.dat
-  Example file path: E:\C\Users\username\AppData\Local\Microsoft\OneDrive\settings\Personal\e4345543.dat
-  E:\C\username\NTUSER.DAT
-  E:\C\$Recycle.Bin\S-1-5-21-XXX-XXX-1002
-  

## Google  

### Location of Interest:  
\Users\<account of interest>\AppData\Local\Google\DriveFS\<account>\metadata_sqlite_db  
You have to say "All Files", there is no extension to the file.  

#### Tools of interest:  
- DB Browser for SQLite  

item_properties table, filter for content-entry (looks for locally cached)  
document item_stable_id  
look at items table for the item_stable_id  
The content-entry of the item_property is protobut format.  Use cyberchef from Hex to Protobuf Decode

- FTK Imager  
File -> Add Evidence -> Image file (.e01)  

- gMetaDataParse
### Location of Interest:  
\Users\<account of interest>\AppData\Local\Google\DriveFS\<account>\metadata_sqlite_db  
Open cache folder: content_cache
Open database: metadata_sqlite_db  
