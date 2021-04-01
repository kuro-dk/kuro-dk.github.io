---
title: 'Mini Synth'
subtitle: 'Hacks & Contraptions'
date: 2017-08-12 00:00:00
description: 
featured_image: '/images/projects/mini-synth/mini_synth.jpg'
---

![](/images/projects/mini-synth/mini_synth.jpg)

Many of my friends are playing with modular synthesizers, and I really like the physical interaction aspect of them. So I wanted to make a small and simple one of my own, trying to make something fast, but at the same time easy to service and take apart, and preferably assembled without the use of glue. I found a simple synthesizer library for Arduino called [Mozzi](https://sensorium.github.io/Mozzi/), and tested it all out on a breadboard. It worked well. I then designed a box for it using a flexbox generator.I have tried to draw it by hand in Illustrator once, and it's just way too much work. I modified the flexbox for my purpose. It takes quite a while to laser cut flex boxes, but they are just way more charming to look at, than a regular tapped box.
I managed to design it all, so that the screws of the panel-mounted USB extension cable I used, keep the whole box together. It works really well, it is a bit fiddly to assemble, but not too bothersome.
This project was made in just a couple of evenings, so I did not test as many things as I should.
There was just enough room for all the components to fit inside of the box, with the panel mounted USB cable ending up rubbing against the speaker. It needed to be trimmed a bit with a scalpel.
The next challenge came when everything was soldered and assembled.

When I was prototyping on the breadboard, I used a Arduino UNO, but when I assembled it, I used an Arduino Pro Micro. The UNO runs on an ATmega328P and the Pro Micro on an ATmega32u4. They both run almost all the same Arduino code, just not the Mozzi library, because of some internal timer differences.
So I ended up having a synthesizer, the only feature of which was that you could change the colour of the LED on top of the box….
Then it was put on the shelf for a month or two, until I got myself together, found another small form factor Arduino, this time a Arduino Nano, and modified the USB extension cable from micro to mini USB.
And finally the it was playing music :D
But… It now has another issue. I can’t control the LED in the way I want, because the synth library uses the timers that were needed to do that, soooo, I'll have to find a fix for that some day.
But it plays nice strange sounds now, which is a lot more satisfying than just an  LED changing colour :)