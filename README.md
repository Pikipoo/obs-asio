# obs-asio
![](/images/obs_icon_very_small.png)  ![](/images/TECH_ASIOsmall.png)

## ASIO plugin for OBS-Studio ##

**Authors** : Andersama (lead) <anderson.john.alexander(a)gmail.com> and pkv <pkv.stream(a)gmail.com>

## Donations
We invested a lot of our time in making this plugin, which we release free of charge.
If you find this plugin useful, consider donating. Even one buck is that much going to buy ourselves a burger !

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=NXB942R9EXY5E&source=url" target="_blank"><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_SM.gif" 
alt="IDonateE"/></a>    

## What is ASIO ? ##
Audio Stream Input/Output (ASIO) is a computer sound card driver protocol for digital audio specified by Steinberg, providing a low-latency and high fidelity interface between a software application and a computer's sound card. Whereas Microsoft's DirectSound is commonly used as an intermediary signal path for non-professional users, ASIO allows musicians and sound engineers to access external hardware directly. (From [ASIO Wikipedia article](https://en.wikipedia.org/wiki/Audio_Stream_Input/Output) ).

## This plugin ##
* We developed a plugin for [OBS Studio](https://obsproject.com/) which is a leading open-source streaming and compositing software.
* It allows capture of ASIO sound devices, which are often professional or semi-professional grade hardware for studio or home-studio use. * The plugin is designed for Windows and has been tested on windows 10 x64.    
* There are five versions but only two are released. They can be found on branches asio-juce, asiobass, asioportaudio, asioportaudio_v2, asiort of this repo.    
  * They use different audio API to host asio drivers (namely JUCE, Bassasio, Portaudio and RtAudio).    
  * The JUCE and Bassasio plugin have the most functionalities; they allow multi-device as well as multi-client operation.    
  * The 2 Portaudio plugins have multi-client but not multi-device capability.
  * The portaudio plugin v2 differs from portaudio plugin v1 in allowing sources with different devices although only one device is active.    
  * The RtAudio based plugin is the most basic one and is not released.     
* Multi-device capability means several asio devices can be used at the same time with OBS Studio. Most applications written with ASIO support including DAW's are limited to one device.
* Multi-client capability means OBS can create several asio sources with different channel selections from the same device.    

## Installation and Usage ##

[Check the wiki](https://github.com/pkviet/obs-asio/wiki/Installation-and-Usage) 
## How to compile and install the plugin ##

[Check the wiki](https://github.com/pkviet/obs-asio/wiki/Compilation-instructions)
