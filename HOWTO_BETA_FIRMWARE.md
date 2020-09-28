# Testing Pre-release Builds of the Tracker firmware

## Before you begin

Hi there! Are you interested in testing beta versions of the next
Tracker firmware?  Great, we're glad to hear that.  Let's just set
some expectations up-front: **beta releases are provided on an "as is"
basis**.  That means any of the following:

* they may introduce new bugs that may lead to loss of work or crashes
  during performance;

* they may introduce new features that will probably not be documented
  before the next stable release;

* they may change or remove previously existing features, both
  documented and undocumented; and

* they may change the data format of the projects or instruments you
  save, making it impossible to open them with an older firmware
  version.

If you find those risks acceptable, let's get you started!

## Download a .ptf file

You can find the latest `.ptf` files in the
[Releases](https://github.com/polyend/TrackerIssues/releases/) section
of this repository.  Note that the "Source Code" in each release doesn't
actually contain Tracker's sources but just this repository's files,
including the one you're reading now.

## Put the .ptf file on your SD card

![SD card view with the Firmware/ folder open](./images/sd-card-firmware.png)

You can use the bundled microSD USB adapter to connect the SD card to
your computer. Put the `.ptf` file in the Firmware/ folder next to other
`.pth` files.
If you erased your card and don't have the latest stable firmware, get
it from [the Polyend website](https://polyend.com/downloads/).

## Put the SD card back in your Tracker and go to Config

![Config/Firmware screen](./images/config-firmware.jpg)

In the Firmware section you'll find a "Firmware update" feature. Enter
it.

## Select the firmware you want

![Firmware selection](./images/config-firmware-selection.jpg)

After selecting the right file, press Select and wait for the upgrade to
finish.  You should see it progress through the file and restart the
device.

## How to get notified about new releases?

If you sign up for GitHub and subscribe to our TrackerIssues repository,
you'll get notified about new releases:

![Watch releases on GitHub](./images/watch-releases-on-gh.png)

You can also sign up for our official
[Polyend Tracker group](https://www.facebook.com/groups/polyendtracker/)
on Facebook.

Finally, you can ask over at https://help.polyend.com/ to be added to
a mailing list notifying of new beta releases.


## If you find bugs

If you're upgrading between beta releases, use the "Reset Config"
feature in the Firmware section of the Config screen. That will ensure

That's why we're testing! Report them
[here](https://github.com/polyend/TrackerIssues).


## In case of serious trouble

If your device lost power during the upgrade, the SD file was damaged,
or the firmware doesn't boot up for any other reason, perform the
emergency flashing procedure as follows:

* download the Polyend Tool from
  [the Polyend website](https://polyend.com/downloads/);

* download a known working firmware file either from the Polyend website
  or one of the previous beta `.ptf` files;

* **important:** remove the SD card from the Tracker; 

* connect your Tracker directly to your computer with a USB cable
  (avoid USB hubs and dongles);

* power up the Tracker;

* in the Polyend Tool, choose the `.ptf` file you want to flash with;

* use a pin to press the hidden Reset button next to the Tracker's
  USB C port;

* wait for the firmware update to complete;

* if it's at 100% but the device didn't reboot on its own, do it
  manually;

* re-insert the SD card to the Tracker's slot.

Still seeing crashes?  Try this: connect your SD card to your computer
and delete the hidden "Workspace" folder.