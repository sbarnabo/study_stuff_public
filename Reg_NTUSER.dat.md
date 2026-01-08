# NTUSER.dat hive  

## Investigation Benefits:  
Find artifacts associated with Evidence of File & Folder Opening such as RecentDocs, OpenSaveMru, and ComDlg32  
Search terms and file paths user typed on the system via TypedPaths and WordWheelQuery keys.  

## Location:  
C:\Users\<useraccount>\ntuser.dat  

## WordWheelQuery  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery (Registry Explorer\WordWheelQuery Plugin Tab)  

#### Value of Note:  
WordWheelQuery does not maintain timestamp, but the timestamp for the key is the last time a value was written.  

## TypedPaths  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\TypedPaths  

#### Value of Note:  
TypedPaths indentifies locations typed by the user into the Windows File Explorer path bar.  
TypedPaths does not maintain timestamp, but the timestamp for the key is the last time a value was written.  

## RecentDocs  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs (Registry Explorer\Recent Documents Plugin Tab)  
#### Value of Note:  
Recent Docs is in MRU order.  The higher the number, the older it is.  The lower the number, the more recent it was accessed.  

## Office File MRU  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Office\16.0\Word\User MRU\ADAL_71509F4C9###\File MRU 

#### Value of Note:  
advantages over the RecentDocs key:  
- full path information  
- timestamps for every entry (which includes "last open" and "last closed"

## OpenSavePidlMRU  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\ComDlg32\OpenSavePidlMRU  


#### Value of Note:  
Most of the files referenced in OpenSavePidlMRU are also present in RecentDocs.  Provides full path information not available in RecentDocs  

## Autostart Run Keys  
### Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Run  

#### Value of Note:  
Registry Explorer has a "bookmark" for this location, and SEVERAL others.  

