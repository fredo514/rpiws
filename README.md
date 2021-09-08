# rpiws
The Raspberry Pi Wireless Speaker

This project is based off the very nice customizable [Super-Simple-Raspberry-Pi-Audio-Receiver](https://github.com/BaReinhard/Super-Simple-Raspberry-Pi-Audio-Receiver-Install), which is sadly no longer maintained. Since it needed to be modified to compile for Buster anyway, I decided to start from scratch and cut the features the Raspberry Pi Wireless Speaker doesn't need.

Why didn't I use Volumio? Initialy because the Bluetooth receiver feature is not free. And also because it's much larger than what the Raspberry Pi Wireless Speaker needs. And what about Sonos or Arylic? These closed source solutions are not customizable and can be shut down anytime. I looked and looked for a simple open source multiroom wireless speaker, but I couldn't find one that does what I needed: A simple open-source multiprotocol audio sink with multiroom sync. And so the Raspberry Pi Wireless Speaker project was started!

The Raspberry Pi Wireless Speaker is a package meant to be installed on a headless Raspberry Pi (Lite OS), to make it into a multiroom wireless speaker. It is meant to be used with my custom amplifier board, the Phile (ADD LINK), but the install script can easily be modified for your own setup.

It provides the following features:
* Bluetooth A2DP sink with volume control
* Airplay sink
* uPnP sink
* AUX input
* S/PDIF input
* Multiroom Sync
* Low-latency bypass
* Web interface
* (future) DSP

Airplay already provides Multiroom Sync for itself. But any of the other sources (Bluetooth, uPnP, AUX, S/PDIF) can be used as Multiroom Sync source too using Snapcast. This means that you can connect to one speaker from your phone as if it were a Bluetooth speaker and have it play on all your snapcast-enabled speakers throughtout your house! The low-latency bypass mode bypasses the snapcast server buffering to provide a better home theater experience.

THIS PROJECT IS STILL A WORK IN PROGRESS.
