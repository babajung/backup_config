Readme.txt

                                                                                
                                                                                
                                                                                
                                                                                
                                                                                
                                                                                
    84454449888094527777          789       782  88888880 788888882 4888888887  
    84590052777                   5887      888 788024407 188414407 8887727888  
    8427                       77 7888     4888 788       288       882    884  
    7      7                  287 78082    8088  88       788       885    888  
     777    7             7 74447 78008   08088 788       288       885    747  
    2  7777           7  2  02247 789084  80088  88       788       885         
     77 77          7 7 4  457247 780088 580088 7887  77  7887  77  885         
    7 72    7    7 7 0  8  022747 7897888887788  88888888 788888885 885         
     57    7 77 2 2 72 24  427257 788 28888 788 7887      788       885         
    8  7  2 77 5 77 87 44  027747 788  8887 588  88       788       885     7   
      7 74  4 72 0  8  58  117247 788  788  488 788       288       885    888  
    77 78  8  8  8  87 207 742747 788   87  488  887      788       881    880  
   72 78  42  8  8  87 704  52247 788       088 788       288       882    884  
     787 787 28  8  88  882  0507 288       888 7887      58852114  8882152888  
     44  48  20  07 707 7247 7447 788       785  88       788888887 4888888887  
                                                                                
   72 2    77  77   7   2         7 7  77   7   7   7  57  7    7  777       8  
   74  477277 077770    8   8 725 27 272 877074 72721  97  572 8 87272 87727 8  
        77  77      7    77  77       727  77      8   777     7 7   7  7  777  
                                                                                
                                                                                
                                                                                
  
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
100.124.0.2 100.124.0.2
Success
Execution Time = 19.697 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-3.txt
100.124.0.3 100.124.0.3
Success
Execution Time = 19.728 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-4.txt
100.124.0.4 100.124.0.4
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
100.124.0.2 100.124.0.2
Success
Execution Time = 19.698 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-3.txt
100.124.0.3 100.124.0.3
Success
Execution Time = 24.937 seconds
===================================[Create path C:\backups\HQ\FL04\ZoneB]===================================
Directory C:\backups\HQ\FL04\ZoneB Existed
===================================[SAVE OUTPUT TO FILE]===================================
C:\backups\HQ\FL04\ZoneB\HQ-FL04B-4.txt
100.124.0.4 100.124.0.4
Success
Execution Time = 19.673 seconds
Total Execution Time = 84.590 seconds

C:\>tree /f backups
Folder PATH listing
Volume serial number is XXXX-XXXX
C:\BACKUPS
├───HQ
│   └───FL04
│       └───ZoneB
│               HQ-FL04B-2.txt
│               HQ-FL04B-3.txt
│               HQ-FL04B-4.txt
│
└───West
    └───FL10
            TA-FL10-1.txt
C:\>
