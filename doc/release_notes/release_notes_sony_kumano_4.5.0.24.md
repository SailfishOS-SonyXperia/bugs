# Sailfish OS 4.5.0.28 for Sony Xperia 1 and 5

These release notes cover Sailfish OS 4.5.0.24 for the following devices:

 - Sony Xperia 1 (J8110, J9110)
 - Sony Xperia 5 (J8210, J9210)

# Intro

This port has been updated last to the latest release of Sailfish OS 4.5.0.24 in addition to that the adaptation to include various security updates and other bug fixes that affect all Sony adaptations taken from Jolla.

Also several documentation updates or buildinfrastructure changes have been made. Most of these updates were fixes to the branching script and
new scripts for release aggregation for update discovery.

The delay between the last release was mostly caused by the development for the update discovery service Cosu and
my personal situation in my private live which had a turn for the worst last year. The Xperia 1/5 II port also took some time of course.

Updates to these project components are now tracking in the main bug tracking repository [SailfishOS-SonyXperia/bugs/releases](https://github.com/SailfishOS-SonyXperia/bugs/releases).

The highlights in this release are:
- [ui] Update submodule to pull in the right icon package for Xperia 1. [SailfishOS-SonyXperia/bugs#37](https://github.com/SailfishOS-SonyXperia/bugs/issues/37)
  The launcher and other icons now should have the right solution
appropriate to the resolution of the device.
- [kernel] Enable CONFIG_EXT4_FS_POSIX_ACL in config. Contributes to JB#59542
- [kernel] free task immediately to prevent slab task_struct memory leak. JB#60580
- [kernel] input: sec_ts: Remove spam from event buffer is empty. Fixes JB#58343
- [kernel] Update to Linux 4.14.264. Fixes JB#59877


*Note the bug numbers have nothing to do with the port directly and are only here for reference*

Thanks to all who have provided testing, reported bugs or have contributed otherwise.

# Functionality

The devices have the same functionality level as the Xperia 10 II port made by Jolla,
except in areas such as VoLTE where public packages are missing or in relation to Sailfish X features which are (currently) unavailable.

# Known issues

* [SailfishOS-SonyXperia/bugs#58](https://github.com/SailfishOS-SonyXperia/bugs/issues/58)
  -  When the phone is unlocked, sometimes there is a bright flash of the screen for a split second (subjectively: for a short split of a second, the screen floods the white background with maximum brightness).
    The issue is triggered rarely and does not cause problems besides a short flash.
* [SailfishOS-SonyXperia/bugs#74](https://github.com/SailfishOS-SonyXperia/bugs/issues/74)
  - The vibration is very short on an incoming call at the very beginning. Then, when there is an incoming call, there is no vibration.
  No workarounds but it shouldn't cause any major impact besides the vibration being to weak notice in many situations.

# Project

The Github project that contains this port and all other ports from this project can be found here:
https://github.com/SailfishOS-SonyXperia

## Project Updates

As explained above there's now a separate changelog for project wide updates which can be found down below:
https://github.com/SailfishOS-SonyXperia/bugs/releases/latest

 The changelog file about the project updates can be found down below:
- [project_changelog.md](https://github.com/SailfishOS-SonyXperia/bugs/releases/download/02-12-2022/project_changelog.md)

## About

The goal of this project is to port additional Sony devices on top of Jolla's existing adaptations while staying as close as possible to the existing ports and contributing back to the upstream where possible.

Most of the changes from Jolla ports are adopted in both directions since the issues that one port has usually apply to the sister device of the same generation (e.g. Xperia 10 II -> Xperia 1/5).
This is the reason why changes from Jolla’s port end up in the changelog for these port,
in many cases because they also affect the specific port but not always.

Where possible changes that were done for this port go back to the _Mer-Hybris_ repositories such as the kernel or droid repositories.

The project is open for anyone that wishes to port additional Sony devices to Sailfish OS. Feel free to suggest new features, provide bug reports or to contribute.

# Report bugs

Bugs can be opened in the bug repository linked below:
https://github.com/SailfishOS-SonyXperia/bugs/

# Download

https://github.com/SailfishOS-SonyXperia/droid-hal-version-sony-kumano/releases/latest


# Flashing

To install Sailfish OS on your device please follow the install instructs in the _flashing-readme.txt_ file included in the archive or read the offical flashing instructions for either the Xperia 10 II or Xperia 10 III:

+ https://jolla.com/sailfishxinstall/

Just make sure to download the software binaries for your device instead of the ones mentioned in the instructions:

+ https://developer.sony.com/file/download/software-binaries-for-aosp-android-10-0-kernel-4-14-kumano-latest

# Changelog

+ [Changelog.md](https://github.com/SailfishOS-SonyXperia/droid-hal-version-sony-kumano/releases/download/4.5.0.28+git1/Changelog.md)
