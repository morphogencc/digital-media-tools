# LIDAR-Lite v3

## Vitals
* Approximate Cost: $150
* Suppliers
    * [Garmin](https://buy.garmin.com/en-US/US/prod557294.html)
* [Operation and Technical Manual](http://static.garmin.com/pumac/LIDAR_Lite_v3_Operation_Manual_and_Technical_Specifications.pdf) -- A link to the datasheet / spec sheet, if it's available.
* Libraries
** Commmunicates via SPI or I2C

## Review
Lidar-Lite is very easy to use; you can interface it with pretty much any microcontroller using SPI or
I2C.  It has a long range of around 40 meters, is very accurate over the entire range, and because it is
laser-based has a very narrow field of view the entire way.

The only downside is that you'll need to use an I2C-to-USB converter to attach it to your computer;
there are a variety of solutions out there, and any sort of modern microcontroller platform can also
accomplish the task.