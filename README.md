# nodejs
this repository contains all the required tools and configurations to setup nodejs for different machines
for MAC, run this: 
# curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -

## Installing the NodeSource Node.js v8.x repo...


## Populating apt-get cache...

+ apt-get update
Get:1 http://security.ubuntu.com trusty-security InRelease [65.9 kB]     
Ign http://archive.ubuntu.com trusty InRelease       
Get:2 http://archive.ubuntu.com trusty-updates InRelease [65.9 kB]
Hit http://archive.ubuntu.com trusty-backports InRelease               
Hit https://deb.nodesource.com trusty InRelease
Hit http://archive.ubuntu.com trusty Release.gpg
Hit http://archive.ubuntu.com trusty Release                               
Get:3 http://security.ubuntu.com trusty-security/universe Sources [75.8 kB]
Get:4 http://archive.ubuntu.com trusty-updates/universe Sources [240 kB]       
Get:5 http://security.ubuntu.com trusty-security/multiverse Sources [3012 B]   
Hit https://deb.nodesource.com trusty/main Sources                             
Hit https://deb.nodesource.com trusty/main amd64 Packages                      
Get:6 http://archive.ubuntu.com trusty-updates/multiverse Sources [7617 B]     
Get:7 http://security.ubuntu.com trusty-security/main amd64 Packages [828 kB]  
Get:8 http://archive.ubuntu.com trusty-updates/main amd64 Packages [1274 kB]   
Get:9 http://security.ubuntu.com trusty-security/restricted amd64 Packages [17.8 kB]
Get:10 http://security.ubuntu.com trusty-security/universe amd64 Packages [237 kB]
Get:11 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3997 B]
Get:12 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [21.1 kB]
Get:13 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [550 kB]
Get:14 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [15.5 kB]
Hit http://archive.ubuntu.com trusty-backports/main Sources                    
Hit http://archive.ubuntu.com trusty-backports/restricted Sources              
Hit http://archive.ubuntu.com trusty-backports/universe Sources                
Hit http://archive.ubuntu.com trusty-backports/multiverse Sources              
Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages             
Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages       
Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages         
Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages       
Hit http://archive.ubuntu.com trusty/universe Sources                          
Hit http://archive.ubuntu.com trusty/multiverse Sources                        
Hit http://archive.ubuntu.com trusty/main amd64 Packages                       
Hit http://archive.ubuntu.com trusty/restricted amd64 Packages                 
Hit http://archive.ubuntu.com trusty/universe amd64 Packages                   
Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages                 
Fetched 3406 kB in 41s (82.0 kB/s)                                             
Reading package lists... Done

## Confirming "trusty" is supported...

+ curl -sLf -o /dev/null 'https://deb.nodesource.com/node_8.x/dists/trusty/Release'

## Adding the NodeSource signing key to your keyring...

+ curl -s https://deb.nodesource.com/gpgkey/nodesource.gpg.key | apt-key add -
OK

## Creating apt sources list file for the NodeSource Node.js v8.x repo...

+ echo 'deb https://deb.nodesource.com/node_8.x trusty main' > /etc/apt/sources.list.d/nodesource.list
+ echo 'deb-src https://deb.nodesource.com/node_8.x trusty main' >> /etc/apt/sources.list.d/nodesource.list

## Running `apt-get update` for you...

+ apt-get update
Hit http://security.ubuntu.com trusty-security InRelease                 
Ign http://archive.ubuntu.com trusty InRelease
Hit http://archive.ubuntu.com trusty-updates InRelease
Get:1 https://deb.nodesource.com trusty InRelease 
Hit http://security.ubuntu.com trusty-security/universe Sources          
Hit http://archive.ubuntu.com trusty-backports InRelease                 
Hit http://archive.ubuntu.com trusty Release.gpg   
Hit http://security.ubuntu.com trusty-security/multiverse Sources              
Hit http://archive.ubuntu.com trusty-updates/universe Sources                  
Get:2 https://deb.nodesource.com trusty/main Sources                           
Hit http://security.ubuntu.com trusty-security/main amd64 Packages             
Get:3 https://deb.nodesource.com trusty/main amd64 Packages                    
Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages       
Hit http://security.ubuntu.com trusty-security/universe amd64 Packages         
Hit http://archive.ubuntu.com trusty-updates/multiverse Sources
Hit http://archive.ubuntu.com trusty-updates/main amd64 Packages
Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages
Hit http://archive.ubuntu.com trusty-updates/restricted amd64 Packages
Hit http://archive.ubuntu.com trusty-updates/universe amd64 Packages           
Hit http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages         
Hit http://archive.ubuntu.com trusty Release                                   
Hit http://archive.ubuntu.com trusty-backports/main Sources                    
Hit http://archive.ubuntu.com trusty-backports/restricted Sources              
Hit http://archive.ubuntu.com trusty-backports/universe Sources                
Hit http://archive.ubuntu.com trusty-backports/multiverse Sources              
Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages             
Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages       
Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages         
Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages       
Hit http://archive.ubuntu.com trusty/universe Sources                          
Hit http://archive.ubuntu.com trusty/multiverse Sources                        
Hit http://archive.ubuntu.com trusty/main amd64 Packages                       
Hit http://archive.ubuntu.com trusty/restricted amd64 Packages                 
Hit http://archive.ubuntu.com trusty/universe amd64 Packages                   
Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages                 
Fetched 6413 B in 16s (394 B/s)                                                
Reading package lists... Done

## Run `apt-get install nodejs` (as root) to install Node.js v8.x and npm
