
# Object Requirements v0.1
## Introduction
For an object to be accepted into the collection, it should comply with the requirements in this documentation The files should be valid, be printable, and the resulting object be usable for it's intended purpose.  Addititonally this document describes which kinds of objects are suitable to be submitted to the collection. 

## Version Control

* **0.1** - this version - initial release

## Acecptable objects

This collection is designed to be a high quality collection of utility objects which are generally useful in the domestic context.  In order to create a useful resource, users must be able to easily understand what kind of objects which this collection contains - this means that not all objects will be suitable for submision. 

Users looking for a wide variety of objects of any kind have other repositories available to them (e.g. Thingiverse, Prusaprinters etc).  However, users looking for practical and useful items for the home can use this collection with confidence that every object in it will be of high quality, likely to produce a good quality printed object. 

### Equality

Objects should be intended for wide use by anyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, religion, or sexual identity and orientation.  The contents of the collection should not enable, or cause, discrimination to any person based on any of these characteristics. Any language used in the object definition (descriptions, titles, etc)  should not assume any of these characteristics of the user.  

Whilst this may be straightforward for most objects, there may be some which are less obvious, for example objects who's utility is specifically linked to a physical characteristic (e.g. sex characteristics) associated with another characteristic.  Extra care must be taken in these cases to ensure that these objects, in their physical form or descriptions adjacent to them in the collection, do not discriminate or assume any characteristics of the user.  

In addition, any contributions are considered on the condition that the contributor follows the [Code of Conduct](CODE_OF_CONDUCT.md).  

### Materials

The material used to print the object may or may not be important, depending on the application.  Objects **must** be able to be printed successfully and be functional using commonly availble 3D printing materials, e.g. ABS, PLA or PETG. The recommended material should be mentioned in the metadata file. Objects which are required to be printed in less common materials to have utility (e.g. flexible filament) should have extra care taken to describe how best to achieve a good result. 

#### Additional Materials
Objects should **preferably** be useful straight from the printer with no additional components. Print-in-place designs are desirable, providing that this does not compromise the utility of the object (i.e. by making it prone to failure).  , Where this is not practical, it is acceptable for additional materials to be specified.  Any additional materials should be common, and ideally standardised (or at least readily available).   

An example of an acceptable additional material may be:
* Metric thread machine head nuts and screws
* Threaded bars
* 5mm steel rods
* 6mm wood dowels

Preferably these materials should be able to be sourced by users in multiple locations around the world. 

#### Tools

In some cases tools may be required to assemble objects.  These tools should be widely available, for example:

* Screw driver (posi, hex, flat)
* Wrench
* Hammer

If more specialised tools are required, consider including a printable version of them with the object to assist assembly. 

#### Fixatives and Adhesives

In some cases, objects might benefit from fixatives to assemble successfully or to improve their robustness.  Ideally, such applications should be optional in preference to mechanical fixings (such as nuts and bolts).  

Where adhesives or chemical formulations are used, they should be readily available in generic forms and as far as possible not specified by brand name (e.g. "medium strength thread locker" rather than "Loctite Threadlocker 243")

### Cost
Objects should be as economical as possible.  The total cost of an individual item should be easily affordable within a single month by someone with an average income. 

### Generality

Objects should be **generally** useful: their usefulness should not be dependent on the user owning any other item.  By specific item, we mean an item which is designed or sold exclusively by a specific supplier.  This does not mean that objects cannot interface with other objects which the user owns - but those interfaces should be standardised or flexible ones rather than bespoke to a specific design. 

An example of a standard interface may be a light switch panel, which has screw holes which are of a standard layout and size on which you can rely. Another example may be a bottle stopper which can fit into bottles with various size openings within a reasonable range. 

### Examples of acceptable and unacceptable objects

Objects that would be suitable could include:

* Clothes pegs
* A hook for a dishcloth
* A cover for a standard 1 gang light switch
* Plant pots
* A spacer clip for 22mm copper plumbing pipes
* A USB plug holder

Objects that would not be suitable:

* Upgrade parts for a specific 3D printer
* A figurine of a character from popular culture
* A clip for an IKEA pegboard (unless it also works with more generic kinds of pegboards)

## Safety

Whilst ultimately the safety of the users of objects in this collection is the responsibility of those users, and no warranty is given, every effort should be made to ensure that no potentially unsafe objects are admitted to the collection.  

Some objects in the home have properties which are critical to their safe operation.  These kinds of objects usually have standards associated with them which specify their properties within certain tolerances.  

As the objects being supplied will be printed by consumers, we cannot guaruntee that any standards for materials, dimensions or other properties will be fulfilled when the object is created.  Therefore, any object for which there are safety critical standards implemented should not be accepted into the collection. 

An example of such an object which is not acceptable for this reason could be a UK 13 Amp domestic plug socket, or a fire alarm cover. 

In some cases objects will be subjected to different environmnetal factors (e.g. moisure, heat or abrasion) which may make some commonly used materials unsuitable for these parts.  In these cases, these objects are still acceptable providing these limitations are clearly stated in the metadata file or README.md file for the object. 

## Printability

Every object in the collection is intended to be printable by the majority of 3D printer owners. 

There is a wide range of capabilities in 3D printers available on the market, however for the purposes of a level playing field, we are expecting that a middle-of-the-road printer accessible to most consumers can be characterised as such:

* A machine of similar quality to [Original Prusa Mini](https://www.prusa3d.com/original-prusa-mini/) or equivilent machine
* A 0.4mm nozzle
* PLA or PETG filament
* A layer height of 0.15mm or greater.
* Which can be completed within 3 hours to an acceptable quality

The print settings required to achieve this must be documented (in the metadata files), and **preferably** photographs showing the result when printed this way also included. 

## Technical Submission requirements

Each object should be submitted as a folder in the `objects` folder at the root of this repository.  Each object must have it's own folder, given a reasonably short name in all lower case alphanumeric characters, with words seperated by `-`.  

An object may consist of several parts, which are subsituted into the filenames below where they reference to `${part}`.  If there is only one part, the part is named after the object itself.

### 3D models

Every object in the collection, by definition, needs a 3D model associated with it.

3D models for the object **must** be stored in a directory called `models`.  

At minimum a [STL format](https://en.wikipedia.org/wiki/STL_(file_format)) file **must** be supplied (as it is currently the most widely supported), but additional formats may also be supplied.  The files should be named as follows:

* [STL format](https://en.wikipedia.org/wiki/STL_(file_format)) - **mandatory** - named `${part}.stl`
* [3MF format](https://en.wikipedia.org/wiki/3D_Manufacturing_Format) - named `${part}.3mf`
* [OBJ format](https://en.wikipedia.org/wiki/Wavefront_.obj_file) - named `${part}.obj`

### CAD sources

Ideally, every object in the collection should be able to be modified and adapted by the users who are able to do so to make them suitable to their specific needs.  Therefore, it is desirable to include 3D CAD source files for each object.

The source for the model **may** also be included in a folder named `source`, in order of preference as below:

* [STEP format (ISO 10303-21)](https://en.wikipedia.org/wiki/ISO_10303-21) - named `${part}.step`
* [IGES format](https://en.wikipedia.org/wiki/IGES) - named `${part}.iges`

### Metadata file
Each object folder **must** contain at least one metadata file in YAML format, in a folder called `metadata` , named `{lang}.yaml`, where {lang} is an [ISO 639-1 language code](https://en.wikipedia.org/wiki/ISO_639-1). There **must** be a `en.yaml` file at minimum. 

The metadadta file should contain the following properties:

* `title` (string): the name of the object - should be a singular noun (e.g. peg, clip, stand).
* `version` (string): a Semantic Version number string for the object. Increment this when you make updates to the object
* `purpose` (string): a single paragraph describing what the object is used for.
* `extra_materials`: (collection, string) a list of additional materials required to assemble the object
* `instructions`: (sequence, string): a set of instructions on how to assemble and use the object once printed, referencing part names as required
* `parts`: (dict, optional): the parts which make up this object (with the key of each relating to the part name). Only required if there are multiple parts
* * `name`: (string) the name of the part
* * `description`: (string) a description of the object
* * `quantity`: (number) the number of these parts which are required to assemble the object
* `license`: (string): the license under which this object is supplied as a [SPDX identifier](https://spdx.org/licenses/)
* `attribution`: (string) any attribution required by the license
* `description`: (string) specifically a physical description of the object once printed (i.e. like a text caption of an image).  **NOT** to be used for general information about the object!
* `suitable_materials`: (collection, string) a list of plastic types which may be suitable for this object to be printed with
* `reference_configuration`: (dict) containing a list of settings used when validating the printability of this object - only specify optional properties if they are critical to the success of the print. 
* * `filament_type`: the type of filament used to print the object.
* * `layer_height`: the layer height set in the slicer
* * `nozzle_size`: the size of the nozzle used for printing in mm
* * `shell_thickness`: (optional) the shell thickness set when slicing
* * `infill_type`: (optional) the type of infill used when slicing
* * `extra_settings`: (optional) any extra slicer settings
* * `post_processing`: (sequence, string, optional): any steps required after the object has completed printing (e.g. removal of supports, freeing hinges)

Property names are alway in English, however the contents must be in the language referenced in the filename.

All prose should be in plain language, using the minimum amount of specialist terminology. Where specialist language must be used, it should be described on the first usage.

### Images
The object **may** be supplied with images to illustrate the object, in a directory called `images`

#### Photographs
An object **may** be supplied with photographs of the object as printed, to illustrate how the object appears when it has been printed with a FDM 3D Printer. 

The object **must** be printed using the slicer settings and hardware documented in the metadata file. 

Each of the photographs **must** be in JPEG format, clearly showing the object on a 100% white background, with an image size of at least 1000 pixels on the shortest side, with the object taking up at least 50% of the size of the image. 

All photos **must** be of the *same object*. 

#### Renders

Computer generated renders **may** be supplied too, conforming with the same specifications as photographs. 

#### Image Files

Images should be stored in the `images` directory, named as follows:

* `${type}-isometric.jpg`: depicting an isometric view of the object
* `${type}-top-down.jpg`: showing the object from the top down
* `${type}-front.jpg`: showing the object from the front in a planar view
* `${type}-side-left.jpg`: showing the object from a different side (rotated 90 degrees clockwise to `${type}-front.jpg`)
* `${type}-back.jpg`: showing the object from a back view (rotated 180 degrees from `${type}-side-1.jpg`)
* `${type}-side-right.jpg`: showing the object from a different side (rotated 270 degrees clockwise to `${type}-front.jpg`)
* `${type}-bottom.jpg`: showing the bottom of the print in plan

Photograph specific files:

* `photo-inuse-${n}.jpg`: showing the object being used - for multiple images increment n. 

In each filename, `${type}` should be replaced with `photo` for photographs, or `render` for 3D computer generated renders.  Images of invividual parts may also be included, with their filename suffixed by `-${part}` before the extension.

Each object does not require all of these photos, and should be submitted in order of preference as the list above. 

### License

Objects may be provided under any license, however that license **must** allow for:

 * Redistribution
 * Derivatives/Remixing

It is desirable for the license to be as unrestricted as possible - however restrictions which do not prevent the above conditions would not result in the object being rejected. Any license must, of course, allow for the object to be added to the collection

Users of the collection should be well informed of the license for each object, which is documented in the metadata file and the README for each object.  

The License for the object **may** also be supplied in a file named `LICENSE.md`.  

#### Examples of accaptable licenses
**[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)** allows for redistribution and derivatives, without any additional restrictions.  

**[GPL 3.0](http://www.gnu.org/licenses/gpl-3.0.html)** allows for redistribution and derivatives of the original. 