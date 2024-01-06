# Lights

I've made a couple of different of types of lights smart and as a result have
used smart bulbs, a couple of different light switches, lamps with integrated
controllers, and smart outlets. 

If you can avoid it, I generally would avoid buying smart bulbs as they require
keeping the switch on // can be accidently turned off easily.

Ultimately, I recommend using Zooz light switches and Sonoff outlets.

## Light Bulbs

### [Philips Hue](https://www.philips-hue.com/en-us)
- I used Philips Hue when I was renting and they're a great gateway into making
your home smart. Two complains, one inherit to all smart bulbs, one to 
California.
  - All smart bulbs require being powered 24/7 for you to send them commands/
  use their smarts. As a result, if you put a smart bulb in a switch controlled
  outlet and someone turns off the switch, the bulb goes offline.
  - Philips has different SKUs for bulbs that can be sold in California because
  of some regulations. The California SKUs do not always go on sale when the
  non-California SKUs go on sale.

## Light Switches

When we bought a home, instead of using smart lightbulbs, we moved to using
smart light switches so that: a) we could use any bulb that fit the socket; and
b) we didn't have to worry about the state of a light switch vis-a-vis the bulb
.

### [Lutron Caseta](https://www.casetawireless.com/)
- We first installed Lutron Caseta switches and they were a good gateway into
smart switches. They use a proprietary radio protocol so you're limited to what
they make.
- My only complaint about them is that they weren't modern toggle switches but
rather were two buttons on a one-gang switch.

### [Zooz Switches](https://getzooz.com)
- We moved and needed scene controllers to control the lights on our Wi-Fi
enabled fans. That resulted in me looking at other switches than Lutron and
landing on Zooz switches and scene controllers.
- Zooz has a relatively complete line of Z-Wave switches and scene controllers,
great wiring diagrams, and high quality hardware.

### [GE Jasco](https://byjasco.com/products/smart-home-automation/z-wave)
- I looked into and used GE Jasco Z-Wave switches before I found Zooz. I
ultimately didn't like the GE Jasco customer service and found their
collection to be less complete than Zooz.

## Smart Outlets

I have a few floor and table lamps that I wanted to make smart and have turn on
with overhead rights. To do so, I connected the lamps to smart outlets and then
have automations in Home Assistant that turn on/off the outlets depending on
the state of different switch controlled lights.

One note about this: this only works for lamps with clear physical switches
that controls power to the lamp. If the lamp has a digital or touch switch, it
likely is drawing power all the time and a smart outlet won't work the way
you want.

### [Sonoff S40ZB Lite](https://sonoff.tech/product/smart-plugs/s40-zb-lite/)
- I use these extensively and like them.

### Wemo Smart Plugs
- I used Wemo smart plugs extensively but the security issues with them and
[Belkins initial decision to not fix them](https://www.theverge.com/2023/5/16/23725290/wemo-smart-plug-v2-smart-home-security-vulnerability)
because they were end of life made me completely move off them.