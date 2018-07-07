# Odd Salon ATEM Macros

## What is this?

This is a configuration dump from my [BlackMagic ATEM](https://www.blackmagicdesign.com/products/atem) 4K ME/1 Switcher. We use the switcher, some cameras, and various SDI/HDMI converters to run our bi-monthly event, _Odd Salon_ (https://www.oddsalon.com). 

Odd salon is produced like a conference. We have a speaker, a laptop, and a need to live-switch slides and views of the speaker in real time. 

We typically connect HDMI1/SD1 to the Laptop (via HDMI), either directly or via a Decimator MD-HX to do frame rate and format conversion. 

SDI2 is connected to the main speaker camera. You can connect the other inputs any way you like, but none of the macros in this configuration will use them.

Of interest to most people will be the `<MacroPool>` section, containing a set of macros to do things like "Put the laptop in the upper corner", or "Put the laptop in the upper right, with speaker in the background." See the macros for more details.

### 2-Up with only one DVE (fake supersource)

I've even included a bit of a 2-Up Cheat. As the ATEM ME/1 only has one DVE to work with, the included graphics template (`odd_salon_2up-dual-mask.psd`) will put the laptop on the left side of the screen, and Camera2 (SDI2) on the right side, through a mask.

Run the "Set up Two-Up" Macro, position the preview camera over the speaker's face, and pull the transition bar (or hit Auto.) It'll seamlessly dissolve into a two-up view which works well for conferences. 

### Installtaion

*This configuration is setup for 1080p/59.94. If you change the size, you might have to change the macro configuration.*

*If your laptop can't output 1080p/59.94, I recommend buying a Decimator MD-HX and using that for format conversion.*

1. Start the ATEM Software Control Software.
1. Back up your Atem first with `File` > `Save As...` 
1. Click `File` > `Restore` and restore the XML file. 

You have the option of selectively restoring parts of the ATEM configuration. You might just want to restore the macros.


