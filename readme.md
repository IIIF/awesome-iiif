# Awesome IIIF

A list of lists of awesome [IIIF](http://iiif.io/) resources

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

## Standards

IIIF has developed several standards.

- [Image API](iiif.io/api/image/)
- [Presentation API](iiif.io/api/presentation/)

## Image Servers

These servers support the IIIF Image API.

- [iiif-image-server-node](https://github.com/jronallo/iiif-image-server-node) written in Coffeescript
- [Loris](https://github.com/loris-imageserver/loris) written in Python
- [IIPImage Server](http://iipimage.sourceforge.net/documentation/server/) high performance image server
- [riiif](https://github.com/curationexperts/riiif) written in Ruby as a Rails engine
- [SIPI](https://github.com/dhlab-basel/Sipi) IIIFv2 image server written in C++

## Image Server Shims

These shims allow you to use an image server that does not currently support IIIF. If you have not implemented an image server yet, this is probably not where you want to start.

- [Djatoka Ruby gem](https://github.com/jronallo/djatoka) convert IIIF URLs into the URLs that Djatoka requires.
- [Shimmy](https://github.com/mejackreed/shimmy) is a Ruby gem designed to help you build shims for the IIIF Presentation API.
- [ContentDM Image translator](https://github.com/IIIF/image-api/tree/master/translators/ContentDM) makes ContentDM images available through IIIF. Python.

## Image Viewers
  - [Universal Viewer](https://github.com/UniversalViewer/universalviewer) is a rich embeddable interface
  - [OpenSeadragon](https://openseadragon.github.io/examples/tilesource-iiif/) has IIIF tile support
  - [Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) lightweight, extensible IIIF image viewer
  - [Mirador](https://github.com/IIIF/mirador) multi-up workspace

## Presentation API Libraries
- [Manifesto](https://github.com/IIIF/manifesto) JavaScript library for both browser and server

## Tutorials

Tutorials for how to accomplish functionality in your applications.

- [IIIF Quick Start Guide](http://iiif.io/technical-details/) is a quick overview of how you might get started with implementing various IIIF standards.
- [Drag and drop](https://medium.com/@aeschylus/create-and-share-iiif-items-quickly-and-easily-with-drag-and-drop-over-email-879f13c9caba) a IIIF image into Mirador

## Implementations

Sites which have implemented IIIF in some respect. Note what standards or other libraries are implemented.

- [Historical State Search](http://historicalstate.lib.ncsu.edu/search) displays images via a IIIF image server.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Jason Ronallo](http://ronallo.com) has waived all copyright and related neighboring rights to this work.
