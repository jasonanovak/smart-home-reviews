
# Cameras and Doorbells

Combining these two categories as there's some ecosystem effects to using
one companies' doorbell and camera offerings.

I ultimately recommend Arlo.

## [Arlo](https://www.arlo.com)
- I've used a series of Arlo cameras --
[Essential Wireless Security Camera](https://www.arlo.com/en-us/cameras/essential/arlo-essential-v2.html),
[Pro 3 Wireless Floodlight Camera](https://www.arlo.com/en-us/light/arlo-pro-3-floodlight-camera.html),
[Pro 4 Wirelss Security Camera](https://www.arlo.com/en-us/cameras/pro/arlo-pro-4.html)
-- and the [Essential Wired Video Doorbell](https://www.arlo.com/en-us/doorbell/video/arlo-wired-video-doorbell.html)
along with their [Secure](https://www.arlo.com/en-us/arlosecure.html) plan.
- I'm happy with the cameras' recording quality, motion detection, and object
recognition.
- The battery life has been good ~6months between recharges.
- The app has a good UX to filter events by triggering event and time,
so if you point them at high traffic areas, you can easily find the events
you want.
- There is not a native Home Assistant integration but the HACS 
[haas-aarlo](https://github.com/twrecked/hass-aarlo) integration does a good
job integrating it into Home Asssistant and making the cameras and their 
sensors available.

## Google Nest
- I've only used the 2nd Gen Google Nest Doorbell (e.g. I have not used the
standalone cameras).
- It didn't integrate with Home Assistant but it does show up on Google Nest
Hubs when someone rang, which was neat.
- I had it pointed at a high traffic area, which meant that it often drained
the battery, even though it was also wired. I solved this by disabling
some recording optoins.

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