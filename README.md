# Project GhostPad

  

**DIFFICULTY:** Intermediate - Advanced
**Status:** Stable Guide (Tested on Lenovo ThinkPad T430)
**Tails Version:** Version 6.18

  

## Overview

  

![enter image description here](https://i.ibb.co/YBFdQJ5k/Project-Ghost.png)

  

*Is privacy even a thing anymore or just a tagline used by companies to harvest and sell your data?*

  

The aim of this project was for me to test the viability of the highest form of security and privacy without going completely off grid and not using electronical devices.

  

## Why This is Useful

  

- **Amnesic Computing** - Without maintaining persistence Tails forgets everything when shutdown.
- **Field-Ready** - Great for journalistis and researchers requiring quick and secure communication.
- **Testing Network Security** - Run Wi-Fi penetration tests without the risk of accidentally keeping sensitive information.

## Hardware Used

- **Laptop:** [Lenovo ThinkPad T430](https://amzn.eu/d/8ttnTVQ)
- **Wi-Fi Adapter:** [TP-Link Archer T2U Nano](https://amzn.eu/d/bDZiMQ3) / USB Hotspot Tethering
- **Tails USB Drive:** [SanDisk 128GB Ultra Flair USB 3.0](https://amzn.eu/d/4Nn6hAb) *(You only really need 32GB but I wanted to have more storage*)
- **Toolkit:** Phillips Screwdriver

## Laptop Specifications

  

- **CPU:** Intel i5-3320M
- **RAM:** 16GB DDR3
- **GPU:** Intel HD Graphics 4000

  

## Laptop Component Removal - T430

  

- Phillips Screwdriver
- Plastic Spudger or Guitar Pick
- Small Container for Screws
- Good Lighting and Uncluttered Workspace
- **Optional:** Anti-Static Wrist Strap

## Power Down & Remove Battery

  

- Shut down the T430 completely and unplug all cables.
- Flip the laptop over.
- Slide the battery release switch to the right whilst sliding the battery upwards.

  
  

## Remove Laptop Storage/SSD

  

- Unscrew the Storage Cover Bay *(Back side of the laptop in the right corner)*
- After unscrewing slowly pry the cover from the laptop.
- Use a screwdriver to grab the two black tabs on either side or use the built in tab to pull the storage out.

  

## Remove Internal Wi-Fi Card

- Look at the back of the device, you should see a rectangular section with two Phillips screws.
- Unscrew these two screws (Keep the screws safe in a storage container)
- You should see two wires which are the Wi-Fi antennas.
- You should notice another screw in this compartment, unscrew it.
- Flip the laptop over and open it up.
- Slowly place pressure on the keyboard and slide it towards the screen. It should pop out of the laptops shell.
- Make sure to not rip the keyboard out as there is a fragile ribbon that can tear during this process.
- Under the keyboard in the middle you should see a small Wi-Fi adapter held in by a single screw. Unscrew it and put back together the laptop.

  

## Remove Webcam & Microphone

  

- Pry open the rim of the display panel, specifically the top portion.
- Remove the small screws holding the camera in place.
- Remove the cable connection to the webcam/microphone (You can cut this out if you dont require it).
- Neatly place the cable back and seal up the shell around the display.

  
  

## Optional: Remove or Disconnect Speakers

If you wish to go above and beyond you can also remove/disconnect the speakers that they can be used by threat actors as microphones as shown [here](https://news.sophos.com/en-us/2016/11/24/how-your-speakers-could-be-turned-into-eavesdropping-microphones/).

  

- Continuing on from removing the Wi-Fi Adapter you will notice two screws above the wrist rest, remove these.
- Pry up the palm rest using your tool of choice.
- The speakers should be located on either side of the laptop, follow each cable and remove it from the motherboard.
- These speakers may also be secured with screws, you can also remove these and pull the speakers out to be extra secure.

  

## Creating a TAILS Bootable USB

  

- Download [Tails](https://tails.net/install/download/index.en.html) from the attached link.
- Download [Rufus](https://rufus.ie/en/) executable.
- Plug in your USB.
- Load Rufus.
- Select Device.
- Click the SELECT button and pick your Tails Image.
- Click Start.
- Wait until it completes and then remove the USB.

  

## BIOS Settings

In this section we will cover how to set the USB as the primary drive along with how to take an additional step to disable certain settings which are useful for privacy.

  

- Plug your USB into the device.
- Press the power button on the Lenovo T430.
- Press F12 multiple times until you are in the boot menu.
- Locate the Boot Mode Settings.
- Use the + or - buttons to move your USB up to the top of the boot queue.

Also an additional thing that you may want to consider is that you may want to disable Secure Boot by navigating to the Security tab and selecting Disable.

  

## First Time Boot

Depending on the Wi-Fi adapter that you have selected you may want to enable Root Permissions by clicking the + icon when loading up Tails and setting a password.

If you don't have a [Wi-Fi adapter](https://tails.net/doc/anonymous_internet/no-wifi/index.en.html) that works out of the box with Tails you can always use your phones hotspot and utilize tethering over USB.

  

## Correct Shutdown Process

Yes it may be aesthetic to simply unplug the USB and watch the system break down whilst spitting out lines of processes. The correct way to shutdown is to like normal, manually shutdown and remove the USB otherwise you are at risk of [Cold Boot Attacks](https://nordvpn.com/cybersecurity/glossary/cold-boot-attack/).

  

## What Youve Achieved

  

- No Internal SSD → No Local Storage Risk
- No Internal Wi-Fi Adapter → Not Tied to MAC Address
- No Webcam/Microphone → Blocks Audio/Video Capture
- No Speakers **(Optional)** → Removes Speaker-as-Microphone Threat

  

## Improvements

If you have any additional improvements that may be useful to increase privacy on this device don't hesitate to reach out to me!

I am aware that my current Wi-Fi adapter isn't natively supported by Tails OS but I intend on buying one of the specified ones soon.

  

## Acknowledgements

  

I would like to acknowledge the YouTube channel GhostStrats for the guidance on how to conduct this project. The tutorials were instrumental on documenting my journey of how to build this device.

  

You can find the channel here: [GhostStrats](https://www.youtube.com/@GhostStrats/featured)
