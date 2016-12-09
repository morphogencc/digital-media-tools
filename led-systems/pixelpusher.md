# PixelPusher0

## Vitals
* Approximate Cost: $120.00
* Suppliers
    * [Illumination Supply](http://www.illumn.com/)
* [PixelPusher Documentation](https://sites.google.com/a/heroicrobot.com/pixelpusher/home)
* Libraries
	* [Java Library](https://github.com/robot-head/PixelPusher-java/) -- also available as a Processing library
	* [C++ Library](https://github.com/morphogencc/ofxPixelPusher)

## Review
PixelPusher is an LED Driver that's pretty ideal for large-scale LED installations.  It connects to your
computer over ethernet (so you don't need USB extenders) and doesn't require any hardware programming --
you simply use the Java or C++ library to send commands to it over UDP and it lights up LEDs as required!

As of the time of this writing, the PixelPusher can be used to control:

* Most LED strips (APA102, WS281*, WS280*, LPD8806) in most combinations of RGBOW
* TLC59711 LED driver chips
* most digital servos

A single pixelpusher also has the ability to push 3840 pixels per pusher, or about 64 meters of the 
standard 60 LEDs / meter type.