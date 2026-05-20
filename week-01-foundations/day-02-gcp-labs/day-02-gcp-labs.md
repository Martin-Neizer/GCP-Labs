			Topic: Compute Engine & Web Server Delpoyment

1. Objective- what was i trying to understand 
## how to rent & Launch a VM in the cloud, 
## install a web server and make it publicly accessable
## and vist its "welcome" page from my own device 

2. Key Concepts (explain terms)

## Virtual Machine VM an iaas device in the cloud
basicaly like having a realy computer with (CPU, RAM, Disk) but it is 
completly software based 

## compute engine iaas
sort of like a rental shop within google cloud where i go to 
look at and design my virtual machines, they manage the hardwear
so that i don't have to 

## External Ip iaas
This is bascally the address of the VM. its like the pubcli street address
and door nuber on the street. if no one has the address they can't find my 
devices on the internet. when i send a request via the internet there 
will be a reterun to sender addres so that i can be found.

## Firewall Rules iaas
This is basically the security gard at the frond gate of  of my houses 
compound, by defult the security grad will not let anyone into the 
compound to visit me unless i have explicitly told them to do so.
"allow HTTP Traffic" port 80 so people can view my website

## Nginx can be iaas, paas, or saas
this i becaiscally the recptionist of my VM (House) It answers the 
foor and shows the website to the visitors 

3. What i did pracitcally 

- created the chepest version of a  VM instance e2-micro
- Enabled HTTP Traffic 
- SSH'd Into the VM via commandline to control the server remotly 
- installed Ngnix (though SSH) i commanded the server to donload and run the web server software
- accessed the external Ip, via a browers to confirm the page was working
- stopped the VM, to prevent google from charging my credit card 

4. Commands i used 
## sudo apt update
to update the list of avaiable software

## sudo apt install nginx -y  
to install the webserver

5. what confused me
using a command line tool to build somthing i can't fully visualise 

6. Mental Model 

- Vm  is the property i just aqquired
- compute engine is the construction company that built the VM instantly 
- External IP is house address for the postman to find
- The FireWall is the locked front gate with a security grad 
- Ngnix is the tennant living insid and says hello when somone knocks 

7. cost awareness 

## when does it charge
- as soon as the vm enters the running state. charges are per-second ( wiht a 1-minuet minimum
## what stops billing 
- stopping the VM pauses the compute charges (engine is off)
but i still pay for the the disk (the storage space i rented)

 **Deleting the VM stops all charges immediately**


