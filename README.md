# Backup files from a server using Onionshare

1) Run connecttoserver.exe as admin on your PC 
2) Run clientstart.exe as admin on the server:
C:\obackup\clientstart.exe --onion http://xdgjlseizutrr65pvast2g26mdxdgjlseizutrr65pvast2g26mduid.onion --folder c:\uploadstuff --regex .* --depth 10 --logfile c:\logfiletext.txt --exitkeys ctrl+x+e --sleepfile 0.1 --sleeprotation 0.1

Explanation: 

### --onion http://xdgjlseizutrr65pvast2g26mdxdgjlseizutrr65pvast2g26mduid.onion 

The server address is generated when you lunch connecttoserver.exe for the first time, it will never change, unless you delete untying-copartner-moonstone.json

### --folder c:\uploadstuff

The folder you want to back up
 
### --regex .*

Regex file filter 

### --depth 10

Max depths of subdirectories 

### --logfile c:\logfiletext.txt

Log file for Exceptions

### --exitkeys ctrl+x+e

Shortcut to kill clientstart.exe since it is headless

### --sleepfile 0.1 

Sleep time between each file 

### --sleeprotation 0.1

Sleep time before next folder scan 

File hashes are saved in C:\Users\USERNAME\AppData\Local\backuplogtmp\backuplogtmp\Cache\backuplog.tmo, and scanned every rotation, if the file has been updated, it will be automatically uploaded
