# Sailfish OS 4.5.0.24 for Sony Xperia 1 II and 5 II

These release notes cover Sailfish OS 4.5.0.24 for the following devices:
- Sony Xperia 1 II (XQ-AT51, XQ-AT52)
- Sony Xperia 5 II (XQ-AS52)

# Intro

This is the first public release of this port. The port existed before it's public release for quite long, it was developed along the Xperia 10 III port.
I'm using it ever since then.  However the testing, polishing and subsequent release took quite some time because of my personal situation and the work on other items such as the the update discovery service Cosu.

The highlights of this release are:

- No notable highlights here exceptthat the device works fully except the known issues
  noted below and the issues where community ports don't have
  the access VoLTE  packages used by Jolla's Sony adaptations.

# Functionality

The devices have the same functionality level as the Xperia 10 III port made by Jolla, except in areas such as VoLTE where public packages are missing or in relation to Sailfish X features which are (currently) unavailable.
Some features such as camera support might be different as for the nature of the difference in platform between the basis of
the two ports (also called boards).


# Known issues

- [sonyxperiadev/bug_tracker#756](https://github.com/sonyxperiadev/bug_tracker/issues/756)
  When trying to record a video the the camera app freezes and has to be forcefully closed.
  The bug is caused by an issue inside the camera server used by the port or the adaptation camera configuration.
  *No workarounds for this issue except to avoid recording videos :/*.

- [sonyxperiadev/bug_tracker#771](https://github.com/sonyxperiadev/bug_tracker/issues/771)
  The recording quality when not using the speakerphone or when calling with the phone to the ear is
  bad that it is hard to hear the user of the device.
  When using the speakerphone the quality of the microphone is slightly better but can
  cause echos.
  *A workaround is a wired or wireless headset.*

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

Most of the changes from Jolla ports are adopted in both directions since the issues that one port has usually apply to the sister device of the same generation (e.g. Xperia 10 III -> Xperia 1/5 II).
This is the reason why changes from Jolla’s port end up in the changelog for these port,
in many cases because they also affect the specific port but not always.

Where possible changes that were done for this port go back to the _Mer-Hybris_ repositories such as the kernel or droid repositories.

The project is open for anyone that wishes to port additional Sony devices to Sailfish OS. Feel free to suggest new features, provide bug reports or to contribute.

# Report bugs

Bugs can be opened in the bug repository linked below:
https://github.com/SailfishOS-SonyXperia/bugs/

# Download

https://github.com/SailfishOS-SonyXperia/droid-hal-version-sony-edo/releases/latest

# Flashing

To install Sailfish OS on your device please follow the install instructs in the _flashing-readme.txt_ file included in the archive or read the offical flashing instructions for either the Xperia 10 II or Xperia 10 III:
- https://jolla.com/sailfishxinstall/

Just make sure to download the software binaries for your device instead of the ones mentioned in the instructions:
  - https://developer.sony.com/file/download/software-binaries-for-aosp-android-11-0-kernel-4-19-edo

#  Updating your device

To update your device please follow the update instructions in INSTALL.org:
[INSTALL.org/Updating your device](https://github.com/SailfishOS-SonyXperia/bugs/blob/master/INSTALL.org#updating-your-device)


# Changelog

+ [Changelog.md](https://github.com/SailfishOS-SonyXperia/droid-hal-version-sony-edo/releases/download/4.5.0.28+git1/Changelog.md)
