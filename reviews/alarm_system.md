# Alarm Systems

Some notes on Alarm Systems:
- There's a lot of options out here including options to make existing alarm
systems smart.
- My requirements were centered around:
  - I wanted a system that would integrate well with Home Assistant;
  - Had remote monitoring;
  - Would let me use the door/window alarm sensors as open/close sensors in
    Home Assistant.
- This combination of requirements meant in practice that I was going to have
to accept a cloud integration for Home Assistant.

Between Simplisafe and Abode, I recommend Abode.

## Simplisafe
- I found that the Simplisafe door sensors were not sensitive enough for my
purposes. I could open the door, go in/out, and close the door without the
sensor registering the door as open.
- I also found their sensor selection lacking vs. Abode.

## [Abode](https://goabode.com)
- Overall I think that this is a good, reliable system.
- My complaints with this system are largely around the behavior of certain
sensors:
  - The glass break sensor is VERY sensitive by default but has dip switches
  you can use to decrease the sensitivity.
  - The water leak sensor is VERY sensitive and VERY loud with no volume
  control, resulting in my [disconnecting the speaker as suggested on reddit](https://www.reddit.com/r/Abode/comments/mitpkm/comment/gt6jhqj/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button&rdt=62170)
  .
- It has a native HomeKit integration that I do not recommend.