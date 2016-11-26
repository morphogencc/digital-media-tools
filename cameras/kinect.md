# Sensor Name

## Vitals
* Approximate Cost: $150
* Suppliers
    * Just about anywhere
* [Datasheet](https://msdn.microsoft.com/en-us/library/jj131033.aspx)
* Libraries
    * [Kinect for Windows SDK](https://msdn.microsoft.com/en-us/library/hh855347.aspx)
* Known Projects:
* Other Resources:

## Constraints

## Review
2d RGB Camera plus a 3d depth image all in one.  Everyone's pretty aware of their capabilities, but some reasons you may want to think twice about using them:

* Limited range (12'-15') and no lensings options (fixed field of view) can make them tricky for applications.
* The driver allows a limited number of them (2 with the original SDK, 3 with a Kinect 2.0 and the new SDK) can be used with a single computer, so you'd need more computers in order to use more than 3 Kinects.