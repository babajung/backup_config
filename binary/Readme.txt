Readme.txt
###############################################################################################################

Command Examples
C:\>py_backup_config_v4.exe –h
C:\>py_backup_config_v4.exe
C:\>py_backup_config_v4.exe -c command.txt -i inventory.csv

###############################################################################################################

C:\>py_backup_config_v4.exe -h
usage: py_backup_config_v4.py [-h] [-v] [-c COMMAND] [-i INVENTORY]
                              [-u USERNAME] [-p PASSWORD]

py_backup_config v4.0
Bancha Sae-Lao <bancha@mfec.co.th>

a tool for backup config and run commands

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         Enable log debugging, default is INFO
  -c COMMAND, --command COMMAND
                        Show-command-list text filename, default is command.txt
  -i INVENTORY, --inventory INVENTORY
                        Inventory csv filename, default is inventory.csv
  -u USERNAME, --username USERNAME
                        Username
  -p PASSWORD, --password PASSWORD
                        Password


###############################################################################################################

C:\>py_backup_config_v4.exe

py_backup_config v4.0
Bancha Sae-Lao <bancha@mfec.co.th>

a tool for backup config and run commands

optional arguments:
  -h, --help            show this help message and exit

Functions:
- Query for every device in inventory file (input csv file of Building/Zone/Floor,IP)
- Generate command to each device
- Create folder for each device (Folder "<base path>/Building/Zone/Floor")
- Save output to individual file (File "<base path>/Building/Zone/Floor/File.txt)

Updated v4:
2019-12-25
- [Done] Add arguments for username and password
- [Done] Change default inventory filename "ip_list_uniq.csv" to "inventory.csv"
- [Done] Measure execution time

Updated v3:
2019-12-02

Updated v2:
2019-11-28
- [Done] Change static "username&password" variables to standard input
- [Done] Change static "show command list" variable to input text file
- [Done] Add logging output to text file
- [Done] Add argument parser for enable/disable log debugging

Username: netadmin
Password:
..Pause..
===================================[Create path C:\backups]===================================
Directory C:\backups Existed
===================================[Create path C:\backups\West\FL10]===================================
Directory C:\backups\West\FL10 Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\West\FL10\TA-FL10-1.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.753 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-2.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.697 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-3.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.728 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-4.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.742 seconds
Total Execution Time = 78.925 seconds

C:\>

###############################################################################################################

C:\>py_backup_config_v4.exe -c command.txt -i inventory.csv

py_backup_config v4.0
Bancha Sae-Lao <bancha@mfec.co.th>

a tool for backup config and run commands

optional arguments:
  -h, --help            show this help message and exit

Functions:
- Query for every device in inventory file (input csv file of Building/Zone/Floor,IP)
- Generate command to each device
- Create folder for each device (Folder "<base path>/Building/Zone/Floor")
- Save output to individual file (File "<base path>/Building/Zone/Floor/File.txt)

Updated v4:
2019-12-25
- [Done] Add arguments for username and password
- [Done] Change default inventory filename "ip_list_uniq.csv" to "inventory.csv"
- [Done] Measure execution time

Updated v3:
2019-12-02

Updated v2:
2019-11-28
- [Done] Change static "username&password" variables to standard input
- [Done] Change static "show command list" variable to input text file
- [Done] Add logging output to text file
- [Done] Add argument parser for enable/disable log debugging

Username: netadmin
Password:
..Pause..
===================================[Create path C:\backups]===================================
Directory C:\backups Existed
===================================[Create path C:\backups\West\FL10]===================================
Directory C:\backups\West\FL10 Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\West\FL10\TA-FL10-1.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 20.278 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-2.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.698 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-3.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 24.937 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-4.txt
100.124.0.1 100.124.0.1
Success
Execution Time = 19.673 seconds
Total Execution Time = 84.590 seconds

C:\>