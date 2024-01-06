# Cameras and Doorbells

Combining these two categories as there's some ecosystem effects to using
one companies' doorbell and camera offerings.

I ultimately recommend Arlo.

## Google Nest
- I've only used the 2nd Gen Google Nest Doorbell (e.g. I have not used the
standalone cameras).
- It didn't integrate with Home Assistant but it does show up on Google Nest
Hubs when someone rang, which was neat.
- I had it pointed at a high traffic area, which meant that it often drained
the battery, even though it was also wired.

## Logitech
- I've used both a series of Logitech Circle cameras and the Circle View
Doorbell.
- They natively supported HomeKit Secure Video, which provides end-to-end
encryption of your video meaning only peopl in your Home can see it.
- Unfortunately the Home.app interface to these cameras was underwhelming
in my experience:
  - It didn't handle cameras with lots of events/recordings well, specifically:
    - It was hard to find specific events from specific days as it required
    scrolling back, waiting for recordings to download, etc.
    - There were events the cameras would miss.
- The Doorbell randomly died one day and it appears to be an issue with the
box Logitech has you connect to the chimes.
- Customer support was not helpful when I needed a replacement mounting bracket
for a camera.

## Arlo
- I've used a series of Arlo cameras and the Arlo wired doorbell.
- My only complaint is that the configuration for new cameras recording when
Home is a bit clunky.
- They don't have native Home Assistant integration but the HACS 
[haas-aarlo](https://github.com/twrecked/hass-aarlo) integration does a good
job integrating it.