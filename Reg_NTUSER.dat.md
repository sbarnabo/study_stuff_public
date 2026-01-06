# NTUSER.dat hive  

## Investigation Benefits:  
Find artifacts associated with Evidence of File & Folder Opening such as RecentDocs, OpenSaveMru, and ComDlg32  
Search terms and file paths user typed on the system via TypedPaths and WordWheelQuery keys.  

## Location:  
C:\Users\<useraccount>\ntuser.dat  

## Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery (Registry Explorer\WordWheelQuery Plugin Tab)  

### Value of Note:  
WordWheelQuery does not maintain timestamp, but the timestamp for the key is the last time a value was written.  

## Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\TypedPaths  

### Value of Note:  
TypedPaths indentifies locations typed by the user into the Windows File Explorer path bar.  
TypedPaths does not maintain timestamp, but the timestamp for the key is the last time a value was written.  

## Registry Location:  
NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs (Registry Explorer\Recent Documents Plugin Tab)  

### Value of Note:  
Recent Docs is in MRU order.  The higher the number, the older it is.  The lower the number, the more recent it was accessed.  
