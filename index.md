# Sonar Sensors

Pros: longer distances (5 - 30 ft), good repeatability, not sensitive to sunlight
Cons: can interfere with each other; using many requires a bit of setup and infrastructure; echoes can be a problem
Neither/Both: Wide beam

## Best Practices

All sonars within line of sight of each other must be triggered simultaneously or one at a time.

## Specific Devices

### Maxbotix Ultrasonic Sensors

# Capacitive Sensors

Capacitive sensors use a human body as a ground to discharge a capacitor plate being charged by the sensor.  They are great for use cases where line of sight cannot be guaranteed (through a barrier), but where accuracy is not required.

Pros: Easy to conceal, no ambient light issues, robust when well tuned
Cons: Tuning can be a pain, Restricted to 0"-24", susceptable to metal objects / EMI

## Best Practices
## Specific Devices

### Roll-Your-Own
This can be done rather cheaply -- read about Delta-Sigma Modulation techniques.

### [Cypress Semiconductor](http://www.cypress.com/capsense/?source=CY-ENG-HEADER)

#### [Jon Moeller's Guide](http://freesoc.net/)


# LIDAR

Summary of LIDAR Sensors

## Best Practices
## Specific Devices

### SICK LMS1xx Series

[Needs editing] Looks like this is good for planar measurements

#### [ofxSick](https://github.com/ZigelbaumCoelho/ofxSick)

### [PulsedLight3D](http://pulsedlight3d.com/)

[Needs editing] Looks like this is ideal for linear measurements

### Kokuyo LIDAR Unit

# Infrared Sensors
Summary of IR Sensors

Pros: Can use many of them without any timing constraints.
Cons: Shorter distance (< 5 ft), sensitive to sunlight and lighting conditions (and black clothes!), minimum sensor range can give false readings, noisier than sonar, non-linear response that should be calibrated
Neither: narrow beam

## Best Practices

Use two IR beams, cross their paths to maximize odds of detecting the object.

## Specific Devices

### Sharp Active IR Sensors
### Passive IR Sensors
### [Panasonic Grid-EYE]()


# Force Sensitive Resistors

## Best Practices
## Specific Devices

# Cameras

Cameras can be used to do much more than proximity detection using CV techniques, and are useful when you need to do something more complex such at object tracking, contour detection, or just tracking of many objects in a large space.

Pros: 2D detection
Cons: More expensive, more computational overhead


## Best Practices
## Specific Devices

### [Rasbperry Pi Camera Board](https://www.adafruit.com/products/1367)
Super cheap, super effective if you need something like 10 fps and simple object detection.

### Thermitrack
### Imaging Source
### Lumenera
### MESA ToF Camera
### Playstation EYE
### Kinect

# RSSI (smartphone, Bluetooth LE beacons)

## Best Practices
## Specific Devices

### [Estimote](http://estimote.com/)
### Bluetooth LE -- Qualcomm Gimbals (blair neal)

#  RFID

While technically a proximity sensor, RFID cannot detect an arbitrary object.  Instead, it's used to detect (and identify) tags that are within proximity of an antenna installed in your exhibit.  A typical use of such device is to detect whether objects have been removed / added to a table.

## Best Practices
Test, test, test your setup!  Nearby metal objects can interfere with the RFID -- be sure to test and calibrate your reader in an environment as close to the production environment as possible.

## Specific Devices

### SM130

The SonMicro SM130 is by far one of the cheapest and simplest readers/antennas you can get (costing about $30 - $40 for a setup), but at a cost -- the detection area is no larger than an index card, the range is limited to 3-6 inches, and it can only read one tag at a time. That said, it's simplicity and cost-effectiveness make it a solid option for many use cases.
