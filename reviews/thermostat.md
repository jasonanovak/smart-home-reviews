# Thermostat

Unless you're doing new construction or can easily run new thermostat wiring,
your smart thermostat option is highly constrained by what wiring you have at
your existing thermostat.

Smart thermostats require continuous power, which means they need a C wire
(or a complicated re-wiring to have an existing wire act as a C wire).

From a user standpoint, I think that the Nest is easier to install and use,
but, the Ecobee is easier to set up in Home Assistant.

## [Nest](https://store.google.com/us/category/nest_thermostats)
- Nest thermostats _don't_ require a C wire, so if you don't have a C wire,
this is the best choice.
- Also of note is that the [Nest Protect smoke detectors](https://store.google.com/us/product/nest_protect_2nd_gen)
work well with Nest thermostats and will do things like "shut off the fan if
smoke is detected".
- The Home Assistant integration for Nest is complicated to set up as it
involves setting up a cloud project and using Cloud APIs. Once set up, it's
stable.
- If you want [Nest Temperature Sensors](https://store.google.com/us/product/nest_temperature_sensor)
or Protect smoke detectors to show up in Home Assistant, you'll to need to use
the [HACS Nest Protect integration](https://github.com/iMicknl/ha-nest-protect).
  - This plugin is annoying to set up but works well and reliably once set up.
- From a privacy perspective, it's worth looking at the 
[Google Nest Security & Privacy Commitments](https://safety.google/nest/)
, which includes descriptions of how Google does and doesn't use data from
Nest devices and sensors. A notable highlight as it is a source of confusion:

      For all our connected home devices and services, we will keep your video
      footage, audio recordings, and home environment sensor readings separate
      from advertising, and we won’t use this data for ad personalization.

## [Ecobee](https://www.ecobee.com/)
- The Ecobee thermostats are most easily set up with a C wire (and, if you
don't have a C wire require complicated re-wiring to _possibly_ have existing
wires act as a C wire).
- The Home Assistant integration is straightforward.