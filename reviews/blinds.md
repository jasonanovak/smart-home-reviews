# Blinds

I have a general preference for top-down/bottom-up cellular shades but those
are difficult (read: expensive) to get in smart configurations.

I think it's hard to go wrong between Hunter Douglas, Ikea, and Yoolax and it's
all a matter of tradeoffs.

## [Hunter Douglas](https://www.hunterdouglas.com/)
- I bought [Hunter Douglas top-down/bottom-up Duette cellular shades](https://www.hunterdouglas.com/window-treatments/shades/cellular-shades)
and, once installed, they're great. 
- "Once installed" is doing a lot of heavy lifting as they are custom order,
which is great for fit/finish but means you have to find a dealer, have
someone come measure, order, have the blinds made, and then have someone come
install them.
- The blinds have BTLE in them so you can control them locally using the
PowerView app on your phone. If you want to integrate them with Home Assistant,
HomeKit, or Google Home  you'll need the hub that bridges BTLE <-> WiFi.
- The current generation of blinds and hub (Gen 3) is not natively supported
by Home Assistant, but the hub exposes HTTP REST endpoints that you can use to
control the blinds. 
- They are quiet.
- They are expensive (~$1300/blind).
- The technical support is excellent.

## [Ikea](https://ikea.com)
- Ikea has a series of [pre-cut smart blinds](https://www.ikea.com/us/en/customer-service/product-support/blinds/)
that are controllable over Zigbee.
- Because they're Zigbee, they're readily added to and controled by
Home Assistant.
- They're a bit noisier than the Hunter Douglas but not annoyingly so.
- They're relatively cheap -- ~$200/blind.
- They're _not_ top-down/bottom-up but will do in a pinch, particularly at
the price.

## [Yoolax](https://www.yoolax.com/)
- I found this brand on [Amazon](https://www.amazon.com/gp/product/B0B1TYPFTS/).
They do custom-cut blinds based on measurements you give them. You're also
responsible for installing them yourself.
- They're relatively cheap -- a 70"w x 40"h blind cost ~$400.
- The top-down/bottom-up blinds I bought have an RF radio in them to control
them remotely. You have to use a [Bond bridge](https://bondhome.io/product/bond-bridge/)
or equivalent to bridge Wi-Fi to RF and control them in Home Assistant.
- The downside to the RF radio + Bond bridge approach is that the motor does
not track the position of the shade, so you have to track this manually in
Home Assistant based upon how long it takes for the shade to go from fully open
to fully closed. 
  - Tracking the position of the shade in Home Assistant means that all 
  open/close actions have to route through Home Assistant.
  - By extension, the RF remote needs to be replaced with a scene
  controller that is programmed to invoke the open/close commands in Home
  Assistant.
  - I've written some [glue code](https://github.com/jasonanovak/smart-home-glue/tree/main/rf_blind_home_assistant_control)
  to automatically track the blind position in Home Assistant.
- They're not actually top-down/bottom-up but rather have a privacy shade
and a blackout shade that goes open -> privacy -> blackout -> closed. You can
have the shade at different states (e.g. 50% light filtering and 50% light
blocking).
- The RF motor is the noisest of the three brands.

## Switchbot
- I tried using two generations of the [Switchbot Curtain](https://us.switch-bot.com/pages/switchbot-curtain)
to automate some existing curtains in my house but found that they were
generally loud, slow, and underpowered.
