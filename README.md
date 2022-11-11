Fork of dockterj/klipper

Adds support for Makerbot Replicator2/2X (Mightyboard rev h and g). 

/config/printer-makerbot-replicator1.cfg can be used as a starting point 
for this printer and i'll be updating it as I go along. 

It follow all the same but removes LED info for the 2 and 2X

TODOs:
* look at capabilities of the on board sd card
* add support for dual extruders
* add documentation for configuring slicers (rep2 specifics)

Installation

Clone this repo and do the normal installation steps.

Copy /config/printer-makerbot-replicator2-2012.cfg to printer.cfg.  Edit this
file to add/remove features specific to your printer (e.g. remove HBP,
change the HBP sensor to match what you have, change x,y, and z limits).

Following the normal installation steps, run make menuconfig.  Choose 
an atmega1280, 16mhz, and uart0.  (see below for note about atmega2560).

Run make flash.  This should flash your mightyboard.  If not, I have
found times where I needed to power the mightboard off and back on
before it would flash.

At this point you should have Klipper running on your Replicator.
Follow the normal Klipper documentation for further tuning.

*************************************************************************
Welcome to the Klipper project!

[![Klipper](docs/img/klipper-logo-small.png)](https://www.klipper3d.org/)

https://www.klipper3d.org/

Klipper is a 3d-Printer firmware. It combines the power of a general
purpose computer with one or more micro-controllers. See the
[features document](https://www.klipper3d.org/Features.html) for more
information on why you should use Klipper.

To begin using Klipper start by
[installing](https://www.klipper3d.org/Installation.html) it.

Klipper is Free Software. See the [license](COPYING) or read the
[documentation](https://www.klipper3d.org/Overview.html). We depend on
the generous support from our
[sponsors](https://www.klipper3d.org/Sponsors.html).
