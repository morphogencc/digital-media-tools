# Thermitrack

## Vitals
* Approximate Cost: $400
* Suppliers
    * [Thermitrack](thermitrack.com)
* [Datasheet](http://www.thermitrack.com/prodinfo.html)
* Libraries
    * [Thermitrack Downloads](http://www.thermitrack.com/downloads.html)
* Known Projects:
    * [Thermitrack Installation Gallery](http://thermitrack.com/installations.html)

## Description
Uses a grid of 4 x 4 thermal sensors to detect blobs underneath the camera, and then uses smart shape-fitting to give high-res coordinates for blob centroids.  This camera is great because it’s cheap enough to throw tons of them across the ceiling to track centroids, and uses thermal imaging, so it’s resilient to noise from radiant IR (e.g. windows and skylights).

One of the bigger drawbacks of using them is that they have a fairly fixed lensing, so you'd need to be able to place them on a fairly regularly grid in order to tile multiples of them.