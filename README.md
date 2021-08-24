# webuzopatch
webuzopatch

This is a hosting control I have tested over and found quite OK. Everything with just one click. 

1. Settings as instructed at the home page: http://www.webuzo.com/wiki/Install

After installation is complete you will find that is using the free version so can not other things like csf , nginx, vanish, .... to do this must be null to become a pretium can install more of these software. 

2. Download the webuzo.php file below and make the correct IP to the IP address you are using and then use ssh up: for example up you to root / directory 

3. run the following command to Get the key: 
 /root/webuzo.php  or   php /root/webuzo.php


- After running the command above, you will see the key code, please copy to a certain txt file and then go through step 4.

4. delete license.php file of 

rm -rf /usr/local/webuzo/enduser/license.php 

create new license.php file 

nano /usr/local/webuzo/enduser/license.php 

Copy key at file license.php. 

Stop the check key from the home page using the following command: 

iptables -A INPUT -s 192.198.80.3 -j DROP 
iptables -A OUTPUT -s 192.198.80.3 -j DROP 
service iptables save 
service iptables restart 

6. Now you log in go back to Webuzo control and see if it's premium
