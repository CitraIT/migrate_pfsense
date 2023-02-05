# migrate_pfsense
Project to Quick Migrate From pfSense firewall to OPNSense With Easy

## usage

1- Install python3.  
2- Install dependencies.  
```
pip -m install --upgrade pip
pip install requests
```  
3- Download this project as .zip or clone it with git clone.  
4- Download the source pfsense config as a backup (menu diagnostics -> backup & restore), rename the downloaded file to pfsense.xml and put aside (same folder) as migrate_pfsense.py script.  
5- Edit the file migrate_pfsense.py and set your OPNSense variables:  
```  
# user defined variables
firewall_url    = 'https://192.168.1.1'
firewall_user   = 'root'
firewall_passwd = 'password'
```  
6- Run the script and watch the screen for processing steps.  
```  
python migrate_pfsense.py
```  
7- That's it! Hope it will help you.
