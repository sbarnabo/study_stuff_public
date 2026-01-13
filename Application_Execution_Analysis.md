# Application Execution Analysis  
## Examples   
- Windows 10 BAM registry key
- NTUSER.DAAT UserAssist key  
- Prefetch Files  

### Useful Tools:  
- Registry Explorer

### Registries Used:  
- NTUSER.dat
- SYSTEM.hve

### Registry Locations (BAM):  
- SYSTEM\ControlSet001\Services\bam\State\UserSettings\SID_of_interest  
#### Notes:  
You can sort by execution time.

### Registry Locations (UserAssist):  
- NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Explorer\UserAssist
- Two most common GUIDs-
-   CEBFF....- Executable file execution
-   F4E57....- Shortcut File Execution
- NTUSER.DAT\Software\Microsoft\Windows\CurrentVersion\Applets\Regedit\LastKey shows last key edited.
  

#### Notes:  
Shows application number of executions, focus times, and last executed date.  

### Prefetch Analysis  
#### WinPrefetch View  
Option \ Advanced Options \ Browse  

pecmd.exe -f theprefetchfile_to_interrogate  
pecmd.exe -d E:\C\Windows\Prefetch -q --csv the_output_location  
Shows run count, the other run times, and files touched  


