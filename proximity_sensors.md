# Sonar Sensors

Pros: longer distances (5 - 30 ft), good repeatability, not sensitive to sunlight

Cons: can interfere with each other; using many requires a bit of setup and infrastructure; echoes can be a problem

Neither/Both: Wide beam

## Best Practices

All sonars within line of sight of each other must be triggered simultaneously or one at a time.

## Specific Devices

### [Maxbotix Ultrasonic Sensors](http://www.maxbotix.com/Ultrasonic_Sensors/MB1000.htm)

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

### [SICK LMS1xx Series](http://www.sick.com/group/EN/home/products/product_news/laser_measurement_systems/Pages/lms100.aspx)

#### [ofxSick](https://github.com/ZigelbaumCoelho/ofxSick)

### [PulsedLight3D](http://pulsedlight3d.com/)

### [Hokuyo LIDAR](https://www.hokuyo-aut.jp/02sensor/index.html#scanner)

### [Velodyne HD Lidar](http://velodynelidar.com/lidar/hdlproducts/hdl64e.aspx)

# Infrared Sensors
Summary of IR Sensors

Pros: Can use many of them without any timing constraints.

Cons: Shorter distance (< 5 ft), sensitive to sunlight and lighting conditions (and black clothes!), minimum sensor range can give false readings, noisier than sonar, non-linear response that should be calibrated

Neither: narrow beam

## Best Practices

Use two IR beams, cross their paths to maximize odds of detecting the object.

## Specific Devices

### [Sharp Active IR Sensors](http://www.sharpsma.com/webfm_send/1208)
### Passive IR Sensors
### [Panasonic Grid-EYE](https://eewiki.net/display/projects/Panasonic+GridEYE+Breakout+Board+and+GUI)


# Force Sensitive Resistors

## Best Practices
## Specific Devices

# Cameras

Cameras can be used to do much more than proximity detection using CV techniques, and are useful when you need to do something more complex such at object tracking, contour detection, or just tracking of many objects in a large space.

Pros: 2D detection

Cons: More expensive, more computational overhead


## Best Practices
## Specific Devices

### [Raspberry Pi Camera Board](https://www.adafruit.com/products/1367)
### [Thermitrack](http://www.thermitrack.com/)
### Imaging Source
### [Lumenera](http://www.lumenera.com/products/surveillance-cameras/index.php)
### [MESA ToF Camera](http://www.mesa-imaging.ch/home/)
### microPlaystation EYE
### Kinect

# RSSI (smartphone, Bluetooth LE beacons)

## Best Practices
## Specific Devices

### [Estimote](http://estimote.com/)
### [Qualcomm Gimbals](http://www.gimbal.com/)

#  RFID

While technically a proximity sensor, RFID cannot detect an arbitrary object.  Instead, it's used to detect (and identify) tags that are within proximity of an antenna installed in your exhibit.  A typical use of such device is to detect whether objects have been removed / added to a table.

## Best Practices
Test, test, test your setup!  Nearby metal objects can interfere with the RFID -- be sure to test and calibrate your reader in an environment as close to the production environment as possible.

## Specific Devices

### [SM130](http://www.sonmicro.com/en/index.php?option=com_content&view=article&id=57&Itemid=70)

The SonMicro SM130 is by far one of the cheapest and simplest readers/antennas you can get (costing about $30 - $40 for a setup), but at a cost -- the detection area is no larger than an index card, the range is limited to 3-6 inches, and it can only read one tag at a time. That said, it's simplicity and cost-effectiveness make it a solid option for many use cases.

### Alien Technology

[API  -- Strings over TCP/IP](http://www.htz.com.tw/products/9800/manual/Reader%20Interface.pdf)

You can also use local ruby scripts to manage read/writes.

Also worth noting -- Alien has a rental program, so for a fee you can rent a reader and try it before you buy it.

### Thinkmagic

[API](http://www.thingmagic.com/images/stories/publicuserguides/MercuryAPI_ProgrammerGuide_Aug12.pdf)

Thinkmagic has excellent partners that will manufacture custom antennas for you.
