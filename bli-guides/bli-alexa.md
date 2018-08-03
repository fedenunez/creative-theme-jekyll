---
title: BeoLiving Intelligence Alexa's skill Guide
layout: pagetoc
---

## Introduction

The scope of this guide comprise a full description of all available voice commands and devices you can control between _Alexa_ and _BeoLiving 
Intelligence_. To enable this feature, remote connection must be enabled in your _BeoLiving Intelligence_ (more information at [BeoLiving Intelligence Quick Setup guide](bli-quick-setup-guide.md)) and  _Alexa_'s skill "_BeoLiving Intelligence skill by Khimo_" must be enabled through _Alexa App_ (refer to [BeoLiving Intelligence Link to Third Party Cloud Service Guide](bli-link-third-party-service.md)). 

**This feature is not upgrade dependent**, so is available in any _BeoLiving Intelligence_ version. If you have not upgraded your _BeoLiving 
Intelligence_ to _PRO_, then all devices apart from _Bang & Olufsen_ devices could not be controlled through _Alexa_.

## Terminology

+ _BeoLiving Intelligence_: Controller with same capabilities as it comes from out of the box.
+ _BeoLiving Intelligence PRO_: Controller with fully capabilities that could offer after upgrading to _PRO_.
+ _BLI_: Alias for BeoLiving Intelligence.
+ _BLI PRO_: Alias for BeoLiving Intelligence PRO.
+ _BLApp_: BeoLiving App.
+ _NL_: Network Link.
+ _LAN_: Local Area Network.
+ _DHCP_: Dynamic Host Configuration Protocol.
+ _HA_: Home Automation.


## Discovery

First step after linking _Alexa_ with your _BLI_ is to discover all devices in your configuration. Automatic discovery of all supported devices is
 done after say "_Alexa, discover my smart home devices_". _Alexa_ will get your _BLI_ configuration and save a reference to all supported 
devices. 

## Device name reference

In the discovery process, _Alexa_ creates a name reference to each device between its zone and name as "_(BLI device zone name)_ \+ 
_(BLI device name)_". For example, to turn on the kitchen light (defined in the zone "Kitchen" and named as "Light" in your _BLI_ configuration) 
you must say "_Alexa, turn on kitchen light_".

## Commands

Supported commands for each device depends in its capabilities. For example, a monochromatic dimmer will not support a set color command.

### Lights/Dimmers

+ Turn on/off: 
  + "_Alexa, turn on/off (LIGHT-NAME)_"
  + Turns on/off light

+ Set brightness: 
  + "_Alexa, dim (LIGHT-NAME) ##%_"
  + Sets brightness level

+ Relative brightness adjust: 
  + "_Alexa, increase/decrease (LIGHT-NAME) by ##%_"
  + Increases/decreases relatively shade level 

+ Set color: 
  + "_Alexa, set the (LIGHT-NAME) to (COLOR)_"
  + Sets light color

## Shades

+ Turn on/off: 
  + "_Alexa, turn on/off (SHADE-NAME)_"
  + Raises/Lowers shade.

+ Set level: 
  + "_Alexa, dim (DEVICE-NAME) ##%_"
  + Sets shade level

+ Relative level adjust: 
  + "_Alexa, increase/decrease (DEVICE-NAME) by ##%_"
  + Increases/decreases relatively shade level 

## Scenes/Macros

+ Activate/Deactivate scene:
  + "_Alexa, activate/deactivate (SCENE-NAME)_"
  + Fires or stops macro

## Themostats

+ Turn off: 
  + "_Alexa, turn off (THERMOSTAT-NAME)_"
  + _Description_: Sets thermostat into Off mode

+ Set thermostat setpoint:
  + "_Alexa, set (THERMOSTAT-NAME) to (TEMPERATURE)_"
  + _Description_: Sets thermostat setpoint to an specific temperature. 
  + _Rules_:
    + In case the thermostat has two setpoints (THERMOSTAT\_2SP _BLI_ resource type) and being in "_Auto_" mode, upper setpoint (Cool setpoint) 
    and lower setpoint (Heat setpoint) will be setted +/- 2 degrees of (TEMPERATURE).     
    + In _Eco_ mode, thermostat setpoints can not be setted.

+ Relative temperature setpoint adjust:
  + "_Alexa, increase/decrease temperature of (THERMOSTAT-NAME)_"
  + _Description_: Increase/decrease thermostat setpoints by a constant value.
  + _Rules_:
    + Same rules than "Set thermostat setpoint" 

+ Set thermostat mode:
  + "_Alexa, set (THERMOSTAT-NAME) to (MODE)_"
  + _Description_: Changes thermostat mode
  + _Rules_: MODE could be any of: "Heat", "Cool", "Off", "Eco" and "Auto"

## Bang & Olfusen NetworkLink devices 

+ Turn on/off: 
  + "_Alexa, turn on/off (DEVICE-NAME)_"
  + _Description_: Turns on device into an specific source or sets into Standby
  + _Rules_: When turning on, selected source can not be predicted. Will be the same for each device.

+ Change channel by number:
  + "_Alexa, change channel to (CHANNEL-NUMBER) on (DEVICE-NAME)_"
  + _Description_: Changes channel by number in current source

+ Change channel by name:
  + "_Alexa, change channel to (CHANNEL-NAME) on (DEVICE-NAME)_"
  + _Description_: Changes channel by name in current source
  + _Rules_: Search for (CHANNEL-NAME) into all favourite lists assigned to device sources. Current source will have priority for a match.

+ Skip channels:
  + "_ Alexa, channel up/down on (DEVICE-NAME)_"
  + _Description_: Changes to next or previous channel in current source
  
+ Set volume:
  + "_ Alexa, set the volume of (DEVICE-NAME) to (VOLUME)_"
  + _Description_: Sets volume level to (VOLUME)
  + _Rules_: Desired volume must be between 0 and 90

+ Relative volume adjust:
  + "_Alexa, turn the volume up/down on (DEVICE-NAME) by (VOLUME-DELTA)_"
  + _Description_: Increase or decrease device volume by (VOLUME-DELTA)

+ Mute/Unmute:
  + "_Alexa, mute/unmute (DEVICE-NAME)_"
  + _Description_: Mute/Unmute device

+ Select source(input):
  + "_Alexa, change the input to (SOURCE-NAME) on (DEVICE-NAME)_"
  + _Description_: Selects source on device. In _Alexa's_ language, "sources" are equivalent to "inputs". Possible sources are all enabled sources on device and manual sources added in _BLI_ _Interfaces_ 
    page (only being _PRO_)

## How to change discovered device name

## Workaround when select input fails

