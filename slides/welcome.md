---
layout: slides
---

[comment]: <> (For a new horizontal slide use: \n===\n)
[comment]: <> (For a new vertical slide use: \n|||n)
[comment]: <> (To write slide notes uses \nNote:)

# BeoLiving Intelligence

===
## BeoLiving Intelligence

#### Comes in 2 flavours:
- BASIC
- PRO

#### 4 times faster than the BLGW

Note:
  - BASIC An entry home controller (From factory) 
  - PRO: BeoLink Gateway  + free remote access + new goodies (must buy an upgrade) 

===
### BASIC (1/2)

- designed for the end-user (Plug & Play)
- fully configurable from the *BeoLiving App*
- Improves security: 
     - password less

Note:
BLI its designed for the end user. Out of the box, could be setted up by some non-technical easy steps.


===
### BASIC (2/2)
 
 
- automatic adds B&O resources
- handle content providers credentials
- product groups
- enable Alexa & IFTTT
- automatic firmware upgrade

Note:
- Some HA systems will be added in the future
- Web interface is completely limited. Network settings, Project info, User management, Firmware upate and Service report are available. Configuration upload/download is not supported.
- Most of the configuration is done through BeoLiving App.


===

## PRO

- The BASIC features
- BeoLink Gateway features
- Remote access configured from factory
- One-time PRO upgarde

Note:
- Paying for a  one-time PRO license upgrade, BLI will unlock the rest of its  capabilities. The way to pay for this license could be done through BLI  BASIC's web interface. In the future is planned to add a way to upgrade  to PRO through BeoLiving App.
- Besides "global" zone, now there is one more default zone called "unassigned-resources" where all NetworkLink devices are added.



===

## What will not work!

- MasterLink devices
- Beo4 and BeoRemote One commands
- Manual soruces
- The admin password


===
## Some features

|||
### Feature: Login without password 

<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/3vyf8GKIrww?autoplay=0&loop=1&playlist=3vyf8GKIrww&start=24"  frameborder="0" height="570" allow="autoplay; encrypted-media" allowfullscreen></iframe>

|||
### Feature: Assign products

<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/9edtGSMGeNg?autoplay=0&loop=1&playlist=9edtGSMGeNg"  frameborder="0" height="570" allow="autoplay; encrypted-media" allowfullscreen></iframe>

|||
### Feature:  Create product groups

<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/VSwNKgSssI8?autoplay=0&loop=1&playlist=VSwNKgSssI8"  frameborder="0" height="570" allow="autoplay; encrypted-media" allowfullscreen></iframe>

|||
### Feature:  Create scenes

<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zpFUk5OeHDg?autoplay=0&loop=1&playlist=zpFUk5OeHDg"  frameborder="0" height="570" allow="autoplay; encrypted-media" allowfullscreen></iframe>

|||
### Feature: Request remote access

<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/9R8mR-LxnXE?autoplay=0&loop=1&playlist=9R8mR-LxnXE"  frameborder="0" height="570" allow="autoplay; encrypted-media" allowfullscreen></iframe>


===
### Alexa tips (BASIC | PRO)

- scenes | create scenes for a improved experience



===


## Thinks to remember

- password "admin" is not valid!
- BASIC from factory
- Khimo cloud from factory
- PRO is compatible with BLGW config


Note:
+ By default, admin user has an unknown password. Inserting button function 2, will set admin password to "admin" for the next 5 minutes. This decision is based in security matters.

===

### Service troubleshooting & Recovery mode guide

- ECON usb to get service report
- Service magic USB to recovery a "DEAD" box

===

### Documentation

- Everything at github
- Help us improving it!
- Send us your github username so we can invite you

|||

### New features for the end user

+ From the APP:
   + Manage zones
   + Assign resouces (NL)
   + Request access to BLI (creates user)
   + Manage products groups
   + Set default credentials of Deezer and TuneIn

|||

### Content provider credentials

+ Possible to set default credentials
+ BLI sets automatically credentials to new devices
+ Previously credentials setting was done manually for each product

Note:
+ Doesn't override existant credentials on devices or sets on devices that previously had
+ Only set credentials when detects a new device without credentials setted

|||

### Products groups

+ Statically link NetworkLink products
+ A product group behaves as one device
+ Same source, same volume in the group
+ Solution for big rooms/installations

Note:
In a products' group, exist a master product that will be the source and volume reference of the group and the rest of the grouped products will follow any source/volume change of master automatically. BeoLiving App will only show the master.

===

### Alexa Skill

Alexa skill is available for BASIC and PRO BLI's, Also, its compatible with BLGW.
With Alexa you can control any standard resource type. 
Examples:
  + Set modes or setpoints of thermostats
  + Select source, change channel, volume control of NetworkLink products
  + Control shades and dimmers
  + Fire scenes

===

### Linking Alexa and IFTTT

Linking process for both cloud services are the same. Linking process starts in their respective apps. Those apps redirects to khimo.com and:
+ A QR code will be displayed that could be scanned through BeoLiving App, if you started the linking process from your pc (as an example).
+ If you are using an iOS device, a button will be shown. After pressing it, BeoLiving App will come up to confirm authorization process.

Khimo User/Password linking process (as it was for IFTTT) is also available as a legacy for BLGW users.

===
### Service troubleshooting & Recovery mode guide

- ECON usb to get service report
- Service magic USB to recovery a "DEAD" box


Note:
These two guides are specially directed to service staff. These describes different complemetary methods to follow in case of malfunction or innappropiate behavior. Besides the common service report procedure, there are two new methods:

+ ECON: consist in attach a USB pendrive named as "ECON" into BLI. BLI will detect when this pendrive is attached and will download to it a big amount of information about BLI current state.
+ Recovery mode: It's possible to boot BLI through a pendrive. This will backup current configuration into the pendrive, will erase current configuration in BLI and download last stable firmware.

