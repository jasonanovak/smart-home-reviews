# Locks

One general note about replacing traditional locks with smart locks: if the
dead bolt is even slightly out of alignment with the strike plate, remotely
locking and unlocking the door will be unreliable.

Exposing a lock from Home Assistant to HomeKit requires exposing it as a
standalone [accessory](https://www.home-assistant.io/integrations/homekit/#accessory-mode)
.

I think that U-Tec and Switchbot solutions are good and recommend them
depending on your needs.

## [U-Tec](https://u-tec.com/)
- The Ultraloq smart lock is manufactured with a variety of wireless options.
I've used the Z-Wave lock.
- Two observations:
  1. The fingerprint sensor requires your finger to be placed precisely on it.
  1. You can't remotely add access codes if you're using Z-Wave.
  
## [Yale](https://www.yalehome.com/)
- I had series of YRD226 locks that I used with Bluetooth and Wi-Fi bridges.
- There was significant lag in locking/unlocking via Home Assistant.

## [Switchbot Smart Lock](https://us.switch-bot.com/pages/switchbot-lock)
- There's one lock that couldn't be replaced and this ended up being a
perfect solution.
- I connected it to Home Assistant using the native bluetooth Switchbot
integration.
- With the right Bluetooth adapter, the connection is repsonsive enough that
locking/unlocking feels instantaneous.
