# Profiling the System through System.hve  
### Establish the CurrentControlSet:  
Record value from SYSTEM\Select\Current key.  
Example: 1 = ControlSet001.  
  
### Document the ComputerName:  
SYSTEM\<CurrentControlSet>\Control\ComputerName\ComputerName  

### Document the TimeZone:  
SYSTEM\<CurrentControlSet>\Control\TimeZoneInformation  

### Last Reboot/Shutdown:  
SYSTEM\<CurrentControlSet>\Control\Windows (Value stored in Windows FILETIME 64-Bit format)  

### Network Interfaces:  
SYSTEM\<CurrentControlSet>\Services\Tcpip\Parameters\Interfaces  
#### DhcpDomain  

### Identify Previously Installed Windows versions  
SYSTEM\Setup\Source OS\  
Keys:  
- ReleaseId
- CurrentBuild
- InstallTime
