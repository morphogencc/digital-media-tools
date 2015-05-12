# Feig MR-102 RFID Reader

## Vitals
* Approximate Cost: $300 - $400
* Suppliers
  * [Digikey](http://www.digikey.lu/catalog/en/partgroup/id-isc-mr102-a-hf/28273)
* [Datasheet](http://www.feig.de/uploads/media/id_isc.mr102_en.pdf)
* Libraries:
* Known Projects:
* Other Resources:
  * Compatible Tag: [TI Tag-it HF-I Pro Inlay](http://www.digikey.com/product-detail/en/RI-I03-114A-S1/481-1088-1-ND/1136198)

## Review

The Feig MR-102 is a mid-price, mid-range RFID Reader that communicates over a variety of communications interfaces.  The same module (using the same API) runs on TCP/IP, USB, or RS-232 (and in both bare-board and enclosed form factors), making it easy to swap between the different versions for different project needs.  It's a good choice for simplicity of use (the library is extremely straightforward) and for needing range (with the FEIG 340/240 Antenna you can get up to 40 cm of range) for a variety of applications.

The MR-102 PoE version is particularly nice because it can be set to a "Notify Mode", where it will automatically forward messages to an IP Address / Port combination whenever the tag status changes.  Otherwise, they have a workable OSX / Windows SDK and Inventorying Software ("IsoStart") to program your tags.

As a bonus, Feig's customer support is top-notch and very professional.  They are extremely responsive and helpful with whatever it is you need.
