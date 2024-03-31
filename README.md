# Smarthome Reviews

I've been interested in the smart home space for a long time and, as I've
moved around, I've smartified a few different homes. As a result, I have some
practical opinions/reviews.

The purpose of this repo is two-fold:
1. Centralize this knowledge for sharing with friends.
1. Reduce the amount of Googling others have to do to answer some of the
questions I had.

## General Notes

There's a lot of different smart home philosophies out there. Mine is
generally:
- Devices should have a failure mode where if the smart home hub is down or
if the Internet is down, the devices should still be usable.
- To the extent possible, controlling my devices shouldn't require a hop
through the cloud.
- Ideally devices aren't using Wi-Fi as their backhaul as I don't want my
Wi-Fi network clogged with devices that don't _really_ need Wi-Fi.
- If devices require an app/login, I want the app/login to support 2FA. This is
a hard requirement for security (camera, locks, etc.) devices.

My smart home journey started with HomeKit but (at the time) I found a lot of
smart home equipment didn't support HomeKit. That led me to [Home Assistant](https://www.home-assistant.io/)
an awesome open source project that acts as a hub and can integrate with ...
almost everything through a rich system of plugins. And, once you have devices
in Home Assistant you can expose them to HomeKit, Google Home, and Alexa.

Currently, my setup is that I have:
- A Raspberry Pi 4 that is booting off an SSD (booting off an SSD is
important as Home Assistant will log alot and wear down an SD Card).
- Z-Wave, Zigbee, and Bluetooth USB sticks connected to the Raspberry Pi
(through USB extension chords as there's too much interference if you 
connect directly to the Raspberry Pi). Specifically, I use a:
  - [Zooz ZST10 Z-Wave stick](https://www.getzooz.com/zooz-zst10-s2-stick/)
  - [Home Assistant SkyConnect Zigbee stick](https://www.home-assistant.io/skyconnect/)
  - [Sena UD100-G03 Bluetooth stick](https://www.amazon.com/gp/product/B0161B5ATM/)
- Home Assistant and ZwaveJS running in Docker containers and the USB sticks
routed to the docker containers.
  - It's relatively easy to do so by mapping the /dev/serial/by-id/X device
to your container.
- After everything is configured in Home Assistant, I expose the devices to
HomeKit and Google Home.
- I subscribe to Nabucasa Cloud to make it easy to expose Home Assistant to
Google home (and to support the Home Assistant project).
- Some of my devices require use of [Home Assistant Community Store (HACS)](https://hacs.xyz/).
- I've added some devices writing some glue code using [hacs-pyscript](https://github.com/custom-components/pyscript/).

## Reviews and Recommendations

- [Alarm Systems](reviews/alarm_system.md) - I recommend Abode
- [Blinds](reviews/blinds.md) - No straightforward recommendation, all
options have tradeoffs
- [Cameras and Doorbells](reviews/cameras_doorbells.md) - I recommend Arlo
- [Ceiling Fans](reviews/ceiling_fans.md) - I recommend Modern Forms
- [Garage Door Openers](reviews/garage_door.md) - I recommend ratgdo
- [Lights](reviews/lights.md) - I recommend Zooz switches and Sonoff outlets
- [Locks](reviews/locks.md) - I recommend U-Tec locks
- [Thermostats](reviews/thermostat.md) - No straightforward recommendation,
all options have tradeoffs
