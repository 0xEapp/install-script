# Yiimp_install_scrypt (update Feb 18, 2018)


Discord : https://discord.gg/w97JMmB

webiste : https://www.alliwantonline.ca

Official Yiimp (used in this script for Yiimp Installation): https://github.com/tpruvot/yiimp


***********************************

## Install script for yiimp on Ubuntu 16.04

After Signing in your VPS =>
- adduser poolname
- adduser poolname sudo
- su - poolname
- git clone https://github.com/emmanuelapp/yiimp_install_scrypt.git
- cd yiimp_install_scrypt/
- sudo bash install.sh (Do not run the script as root)
- sudo bash screen-scrypt.sh 
- sudo bash screen-stratum.sh (configure settings before running this script... adding or removing algos) 

Finish !
Check your domain or server ip in your browser!

###### :NOTE: **DONT FORGET TO  UPDATE THE FOLLOWING FILES BELOW :**
- **/var/web/serverconfig.php :** in order to access the admin panel add your public ip address to this file. 
- **/etc/yiimp/keys.php :** update with API keys from your exchanges for price update and auto exchanging


###### :NOTE: **IMPORTANT** : 

- Your mysql information (login/Password) is saved in **~/.my.cnf**
- **If you reboot your VPS**, you must restart screen-scrypt.sh and screen-stratum.sh (or add crontab)
- Remember to restart **memcached service** after the db change (update or import new .sql)

***********************************

###### This script has an interactive beginning and will ask for the following information :

- Enter time zone
- Server Name 
- Are you using a subdomain
- Enter support email
- Set stratum to AutoExchange
- New location for /site/adminRights
- Your Public IP for admin access
- Install Fail2ban
- Install UFW and configure ports
- Install LetsEncrypt SSL

***********************************

**This install script will get you 95% ready to go with yiimp. There are a few things you need to do after the main install is finished.**

It is your responsibility to fully secure your server. After this installation you may want to make a few changes but most importantly setup  your serverconfig.php file to your liking, add your API keys, and build/add your coins to the control panel. 

There will be several wallets already in yiimp. You can delete them or leave them be theyre included in original yiimp git. 

If you need further assistance send me a message or head over to  discord channel at https://discord.gg/w97JMmB

If this was helpful please help future developments by dontion thanks!! BTC Donation: 1DxxCMNr628ESriH7TEcH1DLhyaasuo9hv
