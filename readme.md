# Awesome IIIF

A list of lists of awesome [IIIF](http://iiif.io/) resources

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

**Disclaimer**: This list is created for informational purposes only and any links do not constitute an endorsement, recommendation, or favoring by the IIIF Consortium.

## Standards

IIIF has developed several standards.

- [Image API](http://iiif.io/api/image/)
- [Presentation API](http://iiif.io/api/presentation/)
- [Content Search API](http://iiif.io/api/search/)
- [Authentication API](http://iiif.io/api/auth/)
- [External Services API Annex](http://iiif.io/api/annex/services/)

## Image Servers

These servers support the IIIF Image API.

- [iiif-image-server-node](https://github.com/jronallo/iiif-image-server-node) written in Coffeescript
- [Loris](https://github.com/loris-imageserver/loris) written in Python
- [IIPImage Server](http://iipimage.sourceforge.net/documentation/server/) high performance image server
- [riiif](https://github.com/curationexperts/riiif) written in Ruby as a Rails engine
- [SIPI](https://github.com/dhlab-basel/Sipi) IIIFv2 image server written in C++
- [RAIS](https://github.com/uoregon-libraries/rais-image-server) 100% open source tile server for JP2 images written in Go
- [digilib](http://digilib.sourceforge.net) image server written in Java
- [Cantaloupe](https://github.com/medusa-project/cantaloupe) image server written in Java


## Image Server Shims

These shims allow you to use an image server that does not currently support IIIF. If you have not implemented an image server yet, this is probably not where you want to start.

- [Djatoka Ruby gem](https://github.com/jronallo/djatoka) convert IIIF URLs into the URLs that Djatoka requires.
- [Shimmy](https://github.com/mejackreed/shimmy) is a Ruby gem designed to help you build shims for the IIIF Presentation API.
- [ContentDM Image translator](https://github.com/IIIF/image-api/tree/master/translators/ContentDM) makes ContentDM images available through IIIF. Python.

## Image Viewers
- [Universal Viewer](https://github.com/UniversalViewer/universalviewer) is a rich embeddable interface
- [OpenSeadragon](https://openseadragon.github.io/examples/tilesource-iiif/) has IIIF tile support
  - [Scalebar Plugin](https://github.com/NIST-ISG/OpenSeadragonScalebar) OpenSeadragon plugin for physical scale overlay
  - [Imaging Helper Plugin](https://github.com/msalsbery/OpenSeadragonImagingHelper) OpenSeadragon plugin with utility functions
- [Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) lightweight, extensible IIIF image viewer
- [Mirador](https://github.com/IIIF/mirador) multi-up workspace
- [Diva.js](https://ddmal.github.io/diva.js/) IIIF image viewer optimized for speed and flexibility

## Presentation API Libraries
- [Manifesto](https://github.com/IIIF/manifesto) JavaScript library for both browser and server
- [Manifesto (UV)](https://github.com/UniversalViewer/manifesto) IIIF Presentation API client and server utility library
- [O'Sullivan](https://github.com/IIIF/osullivan) Ruby API for creating IIIF manifests
- [iiif-prezi](https://github.com/IIIF/iiif-prezi) Python library providing a reference implementation
- [iiif-presentation-api](https://github.com/datazuul/iiif-presentation-api) Java library

## Presentation API Shims

These shims allow you to use systems with presentation metadata (e.g. structure or sequences) that do not currently support IIIF. If you have not implemented the Presentation API yet, this is probably not where you want to start.

- [Shimmy](https://github.com/mejackreed/shimmy) is a Ruby gem designed to help you build shims for the IIIF Presentation API, and has samples for NYPL, Flickr, and the US National Archives.
- [Chronicling America](https://github.com/IIIF/presentation-api/tree/master/translators/chronam) for newspapers digitized in the National Digital Newspaper Program

## Tutorials

Tutorials for how to accomplish functionality in your applications.

- [IIIF Image API live demo](http://yenda.tools/en/iiif-api-demo-en/) Learn about the structure of a IIIF URL through manipulating the parameters and seeing the results in a live demo.
- [IIIF Quick Start Guide](http://iiif.io/technical-details/) is a quick overview of how you might get started with implementing various IIIF standards.
- [Drag and Drop](https://medium.com/@aeschylus/create-and-share-iiif-items-quickly-and-easily-with-drag-and-drop-over-email-879f13c9caba) a IIIF image into Mirador
- [Fellow Travelers: The Canterbury Tales and IIIF](http://web.stanford.edu/group/dmstech/cgi-bin/wordpress/author/blalbrit/) by Benjamin Albritton includes an explanation of the use case for medieval scholars using Chaucer as an example and short section on how to make a page comparison demo in Mirador.

## Slide Decks

Slide decks with a focus on IIIF.

- [OA - Shared Canvas - TEI - Biblissima project](http://www.slideshare.net/biblissima/oa-shared-canvas-tei-biblissima-project) part of a workshop on TEI and neighboring standards including IIIF.

## Discovery

Links to help you discover IIIF resources that have been shared, demonstrations of IIIF discovery and useful discovery tools.

- [iiif-universe](https://github.com/ryanfb/iiif-universe) is a repository that includes links to known IIIF presentation manifest collections.
- [iNQUIRE demo](http://inquire.armtest.uk/) is a demo of an open-source IIIF-compliant research and discovery platform. This is the IIIF-compliant version of the platform driving [Digital Bodleian] (http://digital.bodleian.ox.ac.uk/)
- [iNQUIRE source](https://github.com/armadillo-systems/inquire) is the Github repository for iNQUIRE.

## Implementations

Sites which have implemented IIIF in some respect. Note what standards or other libraries are implemented.

- [Historical State Search](http://historicalstate.lib.ncsu.edu/search) displays images via a IIIF image server.
- [FromThePage](http://www.fromthepage.com) ingests IIIF manifests and displays images for transcription using OpenSeaDragon.
- [SAT Taishōzō Image DB](http://dzkimgs.l.u-tokyo.ac.jp/SATi/images.php?alang=en) by the SAT Daizōkyō Text Database Committee in the DH initiative, the University of Tokyo adopts the IIIF Image and Presentation APIs including over 4,000 annotations displayed on Mirador.

## Experiments and Fun

- [http://puzzle.mikeapps.me/](Puzzles! Powered by IIIF)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Jason Ronallo](http://ronallo.com) has waived all copyright and related neighboring rights to this work.
