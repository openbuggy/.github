# openbuggy
open source software for turning smartphones into vehicles that can be remote controlled in the browser via lte

## buggy
![buggy](https://github.com/openbuggy/.github/assets/19519902/868c9511-add4-471f-b32c-c8f14b500f29)
### parts
- Tamiya Neo Fighter Buggy DT-03 ([amazon](https://www.amazon.de/-/en/TMYTAM58587/dp/B00I92DJNQ))
- Carson CS-6 Steering Servomotor ([amazon](https://www.amazon.de/Carson-500502036-Servo-CS-6-JR-Stecker/dp/B005UDQBX2))
- 2S 5200 mAh Lipo Battery ([amazon](https://www.amazon.de/dp/B0B2DN3KYP))
- Raspberry Pico Microcontroller
- Self built voltage divider for reading battery level with pico
- Samsung S9 with broken glass for 50$ on ebay (way cheaper than raspberry pi with camera, gps, sim etc.)
- OTG adapter to connect phone with microcontroller
- Xbox controller

## web app
![gui](https://github.com/openbuggy/.github/assets/19519902/ea88f87d-52e0-47f8-8c56-24490f7cc4ea)
the web app can be hosted locally or in the cloud. the buggy is controlled with a xbox controller.
[github repo](https://github.com/openbuggy/home)

## android app
the android app connects with the web app via webrtc communicates with the microcontroller via usb. one can also turn on the flashlight. if it's dark. [github repo](https://github.com/openbuggy/app)

## signaling server
to establish a webrtc connection one needs a signaling server. i implemented one in go. [github repo](https://github.com/openbuggy/signaling)

## microcontroller firmware
the firmware of the raspberry pico communicates with the android app via usb and controls the motors via pulse-width modulation. [github repo](https://github.com/openbuggy/controller)

## steering wheel
![wheel-front](https://github.com/openbuggy/.github/assets/19519902/1c0892f0-686a-49a4-891a-0569d8f7de58)
i built a 3d printed steering wheel with a raspberry pico and rotary encoder. in the future, i'll maybe use that instead of the xbox controller. [github repo](https://github.com/openbuggy/steering-wheel)
