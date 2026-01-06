# Registry: Software Profiling  
## Registry Location:  
- SOFTWARE\Microsoft\Windows NT\CurrentVersion

## Values of Note:  
- ProductName
- RegisteredOwner
- ReleaseId
- CurrentBuildNumber
- CurrentBuild
- InstallTime (This value could be initial OS install time, but it could be the last major OS update).
  
## Registry Location:  
- SOFTWARE\Microsoft\Windows NT\CurrentVersion\NetworkList  

## Values of Note:  
"Known Networks" plugin tab (Registry Explorer).  
The key provides a more historical view of network connections than what can be found in the SYSTEM.hve.  
Look at time-frame between "First Connect" and "Last Connect".  

## Registry Location:  
SOFTWARE\Microsoft\Windows NT\CurrentVersion\NetworkList\Signatures\Managed  

## Values of Note:  
Managed networks are typically part of a Windows domain, like a corporate network.  
ProfileGuid info pairs with SOFTWARE\Microsoft\Windows NT\CurrentVersion\NetworkList\Profiles to find: DateCreated, NameType, and DateLastConnected values.  "Known Network" does this work for you.  


## Registry Location:  
SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall
SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall
