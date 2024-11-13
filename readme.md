# Awesome International Image Interoperability Framework (IIIF) [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="https://upload.wikimedia.org/wikipedia/commons/e/e8/International_Image_Interoperability_Framework_logo.png" align="right" width="100">](https://iiif.io/)

A list of lists of awesome [IIIF](https://iiif.io/) resources.

The International Image Interoperability Framework (IIIF - "triple-eye-eff") is a group of standard APIs around sharing and reuse of media. It is also a growing community of galleries, libraries, archives, museums, companies, and others who develop the standards and interoperable software implementations. Content includes helpful links around each of the standards, demonstrations of their use, and tutorials and presentations. The list is especially helpful for orienting new community members and developers.

[![Contributing Guidelines](http://img.shields.io/badge/CONTRIBUTING-Guidelines-blue.svg)](./contributing.md)

## More Resources

The lists below are a great place to start for inspiration and tooling, but they are certainly not complete!

If you have a link or a resource to add, you have a few options: 
- check out the [Contributing Guidelines](./contributing.md) linked just above and submit a pull request yourself if you're familiar with Github worflows
- [open a new issue ticket](https://github.com/IIIF/awesome-iiif/issues/new) mentioning the link or resource you want to add and some description, and the community may be able to help add it

Likewise, there are other ways to see how people are implementing IIIF.
- [Github Topics page](https://github.com/topics/iiif?o=desc&s=updated) - This page will show you the Github repositories that self-identify as IIIF-related, with the most recently updated projects listed first. 
- [IIIF Community on Zenodo](https://zenodo.org/communities/iiif/) - A Zenodo community for gathering articles and data related to IIIF.
- [IIIF on Mastodon](https://julsraemy.ch/mastodiiif/) - People, projects and institutions that self-identify as being active within the IIIF Community on  Mastodon, a federated social network.

**Disclaimer**: The lists below are presented in alphabetical order within each section, and do not suggest any recommendation. Likewise, these lists are created for informational purposes only and any links do not constitute an endorsement, recommendation, or favoring by the IIIF Consortium.

## Contents

- [Standards](#standards)
- [Official Resources](#official-resources)
- [Image Servers](#image-servers)
- [Image Server Shims](#image-server-shims)
- [IIIF Viewers](#iiif-viewers)
- [Image API Libraries](#image-api-libraries)
- [Image Tools](#image-tools)
- [Presentation API Libraries](#presentation-api-libraries)
- [Presentation API Shims](#presentation-api-shims)
- [Presentation Manifest Tools](#presentation-manifest-tools)
- [Validators](#validators)
- [Exhibition and Guided Viewing Tools](#exhibition-and-guided-viewing-tools)
- [Content Search API Servers](#content-search-api)
- [Authentication](#authentication)
- [Tutorials](#tutorials)
- [Videos and Slide Decks](#videos-and-slide-decks)
- [Discovery](#discovery)
- [Annotations](#annotations)
- [Crowdsourcing](#crowdsourcing)
- [Hosting](#hosting)
- [CMS Integration](#cms-integration)
- [Newspapers](#newspapers)
- [STEM](#stem)
- [Experiments and Fun](#experiments-and-fun)
- [Community](#community)
- [Collection Management/Digital Asset Management support](#collection-management-systems-cmss-and-digital-asset-management-dams-that-support-iiif)

## Standards

The IIIF community has developed [several standards](https://iiif.io/api/) for interoperable web-based image delivery.

- [Image API](https://iiif.io/api/image/) - Retrieves images from anywhere in the world and allows the user to select an area of the image and to resize, rotate, and edit the quality.
- [Presentation API](https://iiif.io/api/presentation/) - Packages each image with its metadata so users know the origin, title of the image, and even what page of a book the image was from, likely in conjunction with the Image API.
- [Content Search API](https://iiif.io/api/search/) - Perform search for text within or annotations related to digital objects.
- [Authorization Flow API](https://iiif.io/api/auth/) - Control and restrict access by creating a link to a user interface for logging in and services that provide credentials.
- [Change Discovery API](https://iiif.io/api/discovery/) -  Harvest any changes published by organizations that deliver digital objects.
- [Content State API](https://iiif.io/api/content-state/) - Generate a very specific link to a particular view of an object, like a specific area on a particular page rotated at a certain angle.

### IIIF Extensions

- [navPlace Extension](https://iiif.io/api/extension/navplace/) - This IIIF Presentation 3 API extension defines a new property, navPlace, which is defined by earthbound geographic coordinates in the form of GeoJSON-LD.
- [Georeference Extension](https://iiif.io/api/extension/georef/) - This extension leverages Web Annotations to provide a pattern for georeferencing IIIF Presentation 3 API Canvases as well as Images served through the IIIF Image API, containing (historical) maps.
- [Text Granularity Extension](https://iiif.io/api/extension/text-granularity/) - This extension recommends a pattern for indicating the level of text granularity for an annotation related to optical character recognition (OCR) software, manual transcription, and existing digitized text.

[Feedback is welcome](https://iiif.io/api/#feedback) on all IIIF Specifications, including draft versions and works-in-progress -- please send any feedback to [iiif-discuss@googlegroups.com](mailto:iiif-discuss@googlegroups.com).

## Additional Lists

- [Implementations](https://github.com/IIIF/awesome-iiif/blob/master/implementations.md)

## Official Resources

The [IIIF Consortium (IIIF-C)](https://iiif.io/community/consortium/), with support from the community, maintains a number of resources to assist with understanding and implementation of IIIF.

- [IIIF Cookbook](https://iiif.io/api/cookbook/) - A collection of IIIF "recipes," different reusable code snippets to help create IIIF manifests for common use cases.
- [IIIF Online Workshop](https://training.iiif.io/iiif-online-workshop/) - IIIF workshop materials and videos given by the IIIF-C and updated at each occurrence.
- [IIIF Guides](https://guides.iiif.io/) - A "how-to" resource with screenshots for finding IIIF Manifest URLs from various members of the IIIF community.
- [Image API validator](https://iiif.io/api/image/validator/) - A service to validate a IIIF Image API resource against the specification.
- [Presentation API validator](https://iiif.io/api/presentation/validator/service/) - A service to validate a IIIF Presentation API resource against the specification.

## Image Servers

These servers support the IIIF Image API. Some may also have support for the Presentation API.

- [aws-batch-iiif-generator](https://github.com/vt-digital-libraries-platform/aws-batch-iiif-generator) - An automated pipeline to generate IIIF tiles and manifests and use AWS S3 as an IIIF image server.
- [Cantaloupe](https://cantaloupe-project.github.io/) - Image server written in Java fully conformant to all IIIF Image API versions through 3.0.
- [digilib](https://robcast.github.io/digilib/) - Image server written in Java.
- [FSI Server](https://www.neptunelabs.com/fsi-server/) - FSI Server is a popular commercial solution for serving high resolution images in multiple formats.  It accompanies the Flash-based FSI Viewer for zoom and pan. [IIIF adaptor for FSI server](https://github.com/jhu-digital-manuscripts/rosa/tree/master/rosa-iiif-endpoint)
- [go-iiif](https://github.com/thisisaaronland/go-iiif) - IIIF server written in go (fork of [greut/iiif](https://github.com/greut/iiif)).
- [Hymir IIIF Server](https://github.com/dbmdz/iiif-server-hymir) - IIIF server written in Java supporting IIIF Image and Presentation API.
- [express-iiif](https://www.npmjs.com/package/express-iiif) - Express.js middleware to run an Image API 3.0 compatible IIIF server, written in typescript.
- [iiif_s3](https://github.com/cmoa/iiif_s3) - Ruby library for generating a static IIIF level 0 Image and Presentation API server on Amazon S3.
- [IIPImage Server](http://iipimage.sourceforge.net/documentation/server/) - High performance image server.
- [Loris](https://github.com/loris-imageserver/loris) - Written in Python.
- [Micrio](https://micr.io/iiif) - Commercial platform for hosting IIIF collections with Presentation API support.
- [RAIS](https://github.com/uoregon-libraries/rais-image-server) - 100% open source tile server for JP2 images written in Go.
- [riiif](https://github.com/curationexperts/riiif) - Written in Ruby as a Rails engine.
- [serverless-iiif](https://samvera.github.io/serverless-iiif) - IIIF Image server as an AWS Serverless Application, supporting Image API versions 2.1 and 3.0.
- [SIPI](https://github.com/dasch-swiss/sipi) - IIIFv3 image server written in C++.
- [TremendousIIIF](https://github.com/britishlibrary/TremendousIIIF) - A .NET C# IIIF Image API 2.1 server.


## Image Server Shims

As defined by Wikipedia a shim is a small library that transparently intercepts an API, changing the parameters passed, handling the operation itself, or redirecting the operation elsewhere. These shims allow you to use an image server that does not currently support IIIF. If you have not implemented an image server yet, this is probably not where you want to start. 

- [ContentDM Image translator](https://github.com/azaroth42/pi3f/tree/master/shims/ContentDM) - Makes ContentDM images available through IIIF. Python.
- [Djatoka Ruby gem](https://github.com/jronallo/djatoka) - Convert IIIF URLs into the URLs that Djatoka requires.
- [djiiif](https://github.com/rogerhoward/djiiif) - Package designed to make integrating the IIIF Image API easier by extending Django's ImageField.
- [Flask-IIIF](https://github.com/inveniosoftware/flask-iiif) - Flask extension to support IIIF in Python/Flask applications. See [Flask-IIIF previewer demo](http://flask-iiif.herokuapp.com/previewer) and [Flask-IIIF RESTful demo](http://flask-iiif.herokuapp.com/restful).
- [Shimmy](https://github.com/mejackreed/shimmy) - Ruby gem designed to help you build shims for the IIIF Presentation API.

## IIIF Viewers

- [Allmaps](https://https://allmaps.org/) – A set of tools for curating, georeferencing and exploring IIIF maps.
- [Archive Viewer](https://archiveviewer.org/) - A viewer for scanned images from various archives and repositories. (Presentation API v2 only)
- [CanvasPanel](http://canvas-panel.netlify.com/) - React library to build IIIF Presentation 3 level viewing experiences including support for annotations.
- [Chronoscope World](https://mprove.de/chronoscope/world.html) – A viewer for georeferenced IIIF maps. It is also a fast viewer for browsing IIIF books.
- [Clover IIIF Viewer](https://samvera-labs.github.io/clover-iiif/docs/viewer) – Presentation API Manifest and Collection viewer handling Image, Sound, and Video canvases for React.js
- [Diva.js](https://ddmal.github.io/diva.js/) - IIIF image viewer optimized for speed and flexibility.
- [Glycerine Viewer](https://github.com/Systemik-Solutions/glycerine-viewer) - An elegant and contemporary Vue 3 Viewer with a comprehensive annotation feature set.
- [IIIF Curation Viewer](http://codh.rois.ac.jp/software/iiif-curation-viewer/) - A general IIIF viewer with added focus on curation and ordering of cropped IIIF images. [Demo](http://codh.rois.ac.jp/software/iiif-curation-viewer/demo/?curation=https://gist.githubusercontent.com/2SC1815J/18e1228c52a6650c64902142ed7496f8/raw/7a247b64b6e22357e83f573b7283e31f3111af68/curation_kibutsu.json&pos=4)
- [Internet Archive BookReader](https://github.com/internetarchive/bookreader) - A viewer developed by the Internet Archive, specially suited for viewing books.
- [Micrio](https://micr.io/iiif) - High-performance client with WebAssembly/WebGL engine and additional storytelling elements. Also offering full server IIIF support.
- [Mirador](projectmirador.org/) - Multi-up workspace. See also [Awesome Mirador list](https://github.com/ProjectMirador/mirador-awesome).
- [Tify](https://github.com/subugoe/tify) - Slim and fast IIIF document viewer built with Vue.js.
- [Universal Viewer](universalviewer.io/) - Rich embeddable interface.

### Image viewers (Image API only)

- [OpenSeadragon](https://openseadragon.github.io/examples/tilesource-iiif/) - IIIF tile support.
  - [Scalebar Plugin](https://github.com/NIST-ISG/OpenSeadragonScalebar) - OpenSeadragon plugin for physical scale overlay.
  - [Curtain Viewer](https://github.com/vanda/curtain-viewer) - Viewer based on OpenSeadragon using the curtain-sync plugin for comparing naturally aligned image variants
- [openseadragon-react-viewer](https://www.npmjs.com/package/openseadragon-react-viewer) - A React wrapper component around OpenSeadragon which offers selectable, extended UI functionality.
- [IIIFViewer](https://github.com/klokantech/iiifviewer) - IIIF WebGL / Canvas / DOM mobile-ready fast viewer powered by OpenLayers V3.
- [Imaging Helper Plugin](https://github.com/msalsbery/OpenSeadragonImagingHelper) - OpenSeadragon plugin with utility functions.
- [IIPMooViewer](https://iipimage.sourceforge.io/documentation/iipmooviewer/) - IIPMooViewer is an open source, Javascript and HTML5 image streaming and zooming client. IIPMooViewer is IIIF-compatible and works with IIPServer or other IIIF compatible servers. [Demo](https://iipimage.sourceforge.io/demo/)
- [Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) - Lightweight, extensible IIIF image viewer.
- [OpenLayers](https://openlayers.org) - High-performance, feature-packed Javascript library especially built for maps. It supports the IIIF Image API 2.1.

## Image API Libraries

- [iiif](https://github.com/zimeon/iiif) - Python library providing a reference implementation of the Image API. Also includes a test server and static tile generator.
- [iiif-apis](https://github.com/dbmdz/iiif-apis) - Java IIIF API libraries.
- [iiif_url](https://github.com/NCSU-Libraries/iiif_url) - Ruby library for creating and parsing IIIF Image API URLs.
- [iiif-tiler](https://github.com/glenrobson/iiif-tiler) - Java library for generating static IIIF tiles (compliant with the V2.1 and 3.0 of the IIIF Image API). 
- [image-iiif](https://github.com/conlect/image-iiif) - A bring your own framework solution for implementing IIIF Image API 2.1 with PHP.
- [iOSTiledViewer](https://github.com/moravianlibrary/iOSTiledViewer) - IIIF image API and Zoomify viewer for iOS, written in Swift.
- [libvips](https://libvips.github.io/libvips/) - A fast image processing library with low memory needs. Includes an operation that can build image pyramids compatible with IIIF Image API.
- [Node node-iiif](https://github.com/samvera/node-iiif) - a full-featured image processor supporting the IIIF Image API versions 2.1 and 3.0.
- [piffle](https://github.com/emory-lits-labs/piffle) - Python library for generating and parsing IIIF Image API URLs.

## Image Tools

Various tools for working with images such as cropping tools.

- [CanvasFinder](https://glenrobson.github.io/CanvasFinder/) - allows you to paste a IIIF Manifest URL into the box below and it will show you all of the Canvases which are present in that manifest.
- [Compariscope](https://vanda.github.io/iiif-features/) - A demo app by the Victoria & Albert useful for the alignment of overlayed images, served by the IIIF Image API, and providing an interactive viewer for overlayed images, presented fluidly, using responsive image tags.
- [dezoomify-rs](https://github.com/lovasoa/dezoomify-rs) - A command-line tiled image downloader. Support IIIF, Deepzoom and others zoomable image formats.
- [IIIF cropping tool](https://ncsu-libraries.github.io/iiif-crop-tool/) - Website using [Leaflet-IIIF Cropping](https://bl.ocks.org/mejackreed/6936585f435b60aa9451ae2bc1c199f2) and Jekyll that allow users to enter the URL of a IIIF image and get the URL for the cropped section of the image.
- [iiif-dl](https://github.com/ryanfb/iiif-dl) - Command-line tile downloader/assembler for IIIF endpoints/manifests. Download full-resolution image sequences from any IIIF server.
- [IIIF Image Inspector](https://iiifimage.link/) - a small tool to inspect metadata about IIIF images and demonstrate how their image file URLs may be constructed.
- [IIIF-imageManipulation](https://github.com/jbhoward-dublin/iiif-imageManipulation) - UCD's tool to crop images and manipulate via IIIF attributes; integrate with Mirador via plugin.
- [Leaflet-IIIF Cropping](https://bl.ocks.org/mejackreed/6936585f435b60aa9451ae2bc1c199f2) - Example of using Leaflet to provide IIIF cropping.
- [Software tools from Oxford Visual Geometry Group](https://www.robots.ox.ac.uk/~vgg/software/)

## Presentation API Libraries

- [IIIF Manifest Generator](https://github.com/yale-web-technologies/IIIF-Manifest-Generator) - PHP library for generating IIIF manifests.
- [iiif-apis](https://github.com/dbmdz/iiif-apis) - Java IIIF API libraries.
- [iiif-prezi](https://github.com/iiif-prezi/iiif-prezi) - Presentation 2 Python library providing a reference implementation.
- [iiif-prezi3](https://github.com/iiif-prezi/iiif-prezi3) - Presentation 3 Python library.
- [iiif-tree-component](https://github.com/edsilv/iiif-tree-component) - IIIF tree menu sortable by date with multi-select capability.
- [jiiify-presentation](https://github.com/ksclarke/jiiify-presentation) - A Java IIIF Presentation library.
- [Manifesto](https://github.com/UniversalViewer/manifesto) - IIIF Presentation API client and server utility library.
- [Manifold](https://github.com/UniversalViewer/manifold) - Wraps Manifesto to provide viewer state and related utilities.
- [Clover IIIF](https://samvera-labs.github.io/nectar-iiif/) - IIIF front-end React toolkit including a multimedia viewer, image slider, and HTML5 primitives for manifest properties.
- [O'Sullivan](https://github.com/IIIF/osullivan) - Ruby API for creating IIIF manifests.
- [pyIIIFpres](https://github.com/giacomomarchioro/pyIIIFpres) - A Python module built for easing the construction of JSON manifests compliant with IIIF API 3.0 in a production environment, similarly to iiif-prezi for earlier versions of the protocol.
- [Swiiift](https://github.com/mejackreed/Swiiift) - IIIF presentation API library for Swift.
- [tabula-rasa](https://www.npmjs.com/package/tabula-rasa) - npm module for creating and manipulating IIIF manifests.
- [tiny-iiif-manifest-authoring-tool](https://github.com/yuta1984/tiny-iiif-manifest-authoring-tool) - A node.js web app that provides a one-stop solution for publishing IIIF resources, offering various functionalities from image uploading to IIIF manifest authoring.
- [ViewDir](https://iiif-commons.github.io/) - Documentation on IIIF-related libraries and components, from an open community of designers and developers interested in creating composable and interoperable interfaces for consuming and creating online content.

## Presentation API Shims

These shims allow you to use systems with presentation metadata (e.g. structure or sequences) that do not currently support IIIF. If you have not implemented the Presentation API yet, this is probably not where you want to start.

- [Chronicling America](https://github.com/azaroth42/presentation-api-shims/tree/master/shims/chronam) - For newspapers digitized in the National Digital Newspaper Program.
- [Shimmy](https://github.com/mejackreed/shimmy) - Ruby gem designed to help you build shims for the IIIF Presentation API, and has samples for NYPL, Flickr, and the US National Archives.

## Presentation Manifest Tools

- [biiif](https://github.com/edsilv/biiif/) - Organise your files according to a simple naming convention to generate IIIF v3 manifests.
- [demetsiiify](https://github.com/jbaiter/demetsiiify) - Web service for creating IIIF manifests from METS/MODS documents.
- [IIIF Download](https://www.lizmfischer.com/iiif-tools/download) - Input a IIIF Manifest URL to and the desired image size to download a zip of all that Manifest's images
- [IIIF Manifest Explorer](https://www.lizmfischer.com/iiif-tools/manifest) - Input a IIIF manifest link to see basic object and image metadata in a human-friendly format.
- [iiif-producer](https://github.com/ubleipzig/iiif-producer) - A CLI tool that generates IIIF Presentation 2.1 Manifests from METS/MODS (produced by Kitodo).
- [Leiden's Islandora IIIF Manifest Generator](https://github.com/LeidenUniversityLibrary/islandora_iiif_manifests) - A module to generate IIIF Manifest for Islandora.
- [Manifest Editor](https://github.com/bodleian/iiif-manifest-editor) - Web application for importing, viewing, updating, and exporting manifests. See a [demo](https://digital.bodleian.ox.ac.uk/manifest-editor/).
- [Brif](https://github.com/pierrz/brif) - A boilerplate tool based on Docker and FastAPI, designed to streamline the development and deployment of IIIF compliant platforms. Powering up muzai.io. See live [demo](https://brif-demo.muzai.io/dashboard).
- [pdiiif](https://github.com/jbaiter/pdiiif) - a JavaScript library to create PDFs from IIIF manifests, completely client-side (with server-based fallback for unsupported browsers). 
- [tropiiify](https://github.com/martimpassos/tropiiify) Tropy plugin that exports images, metadata and annotations as a (level0) IIIF collection. 

## Validators

- [Presentation API validator](https://iiif.io/api/presentation/validator/service/) - A service to validate a IIIF Presentation API resource against the specification.
- [Image API validator](https://iiif.io/api/image/validator/) - A service to validate a IIIF Image API resource against the specification.
- [Hyperion](https://www.npmjs.com/package/@hyperion-framework/validator) - IIIF Presentation API 3 Validator in JavaScript [N.B. being replaced by [Vault](https://github.com/IIIF-Commons/vault) as part of the [IIIF Commons](https://github.com/IIIF-Commons/)]
- [Tripoli](https://ddmal.github.io/tripoli/) - IIIF Presentation API 2.0+ validation library.

## Exhibition and Guided Viewing Tools

Tools and resources that provide functionality for presenting IIIF materials in an exhibition-like setting (and potentially other functionality).

- [Adno](https://adno.app/en/) - a web application for viewing, editing and sharing narratives and pathways on IIIF images.
- [Annona Range Storyboard](https://ncsu-libraries.github.io/annona/range/) - [Annona](https://ncsu-libraries.github.io/annona/) toolkit which allows for the guided viewing of segments of a manifest, in addition to the [Annona Multi Storyboard Viewer](https://ncsu-libraries.github.io/annona/multistoryboard/) for guided comparison of multiple manifests.
- [Canopy IIIF](https://github.com/mathewjordan/canopy-iiif) - A IIIF Collection sourced site generator in Next.js for digital collections, humanities, and exhibitions 
- [Curation Tools](http://codh.rois.ac.jp/software/) - Set of tools, including a Viewer, Curation Manager, Curation Board, and more from the Center for Open Data in the Humanities (all tool descriptions in Japanese, some also available in English).
- [Exhibit](https://exhibit.so/) - A free IIIF storytelling tool that allows for guided navigation of one or more IIIF Manifests using annotations.
- [Micrio](https://micr.io/iiif) - High-performance client with WebAssembly/WebGL engine and additional storytelling elements. Also offering full server IIIF support.
- [Juncture](https://www.juncture-digital.org/) - a suite of tools and services that enable anyone to easily create engaging web pages with rich visualizations, including interactive images, videos, maps, and more.
- [Panel Truck](https://geoservices.leventhalmap.org/cartinal/documentation/panel-truck.html) - Vue-based presentation tool, embeddable into any page as a Web Component, which supports slide-like narration over one or multiple IIIF sources, as well as static images and tiled map sources. ([Example](https://geoservices.leventhalmap.org/panel-truck/example.html))
- [Simple Site IIIF Extensions](https://jpadfield.github.io/simple-site/extensions.html) This [Simple Site](https://jpadfield.github.io/simple-site/) has several extensions that make use of IIIF to produce customised presentations of a bespoke selection of IIIF manifests (e.g. in Mirador 3, Curtain Viewer and Panel Truck).
- [Spotlight](http://spotlight.projectblacklight.org/) - a self-service approach for creating exhibit websites to highlight digital collections; based on [Blacklight](http://projectblacklight.org/).
- [Storiiies Editor](https://storiiies-editor.cogapp.com/) – a free online storytelling platform for creating guided tours of a single IIIF manifest using annotations.
- [Wax](https://minicomp.github.io/wax/) - a minimal computing project for producing digital exhibitions focused on longevity, low costs, and flexibility.


## Content Search API

Libraries and applications that support the Content Search API.

- [Blacklight IIIF Search](https://github.com/boston-library/blacklight_iiif_search) - Plugin that provides IIIF Content Search functionality for [Blacklight](https://github.com/projectblacklight/blacklight)-based Rails applications.
- [Ocracoke](https://github.com/NCSU-Libraries/ocracoke) - Rails application to create, index, and search text from page images and provide results in IIIF Content Search API format.
- [Whiiif](https://github.com/mbennett-uoe/whiiif) - Python/Flask/Solr application to index IIIF manifests alongside ALTO representations and provide a IIIF Content Search API endpoint.

## Authentication

Some resources about the IIIF Authorization Flow API.

- [IIIF Auth Demonstrator](https://tomcrane.github.io/iiif-auth-client/?collection=https://iiif-auth2-server.herokuapp.com/collection.json) - Manifests with accompanying images and AV resources that demonstrate various IIIF authentication patterns.
- [iiif-auth-client](https://github.com/tomcrane/iiif-auth-client) - Client implementation of the IIIF Authorization Flow specification.
- [iiif-auth-server](https://github.com/tomcrane/iiif-auth-server) - A demo server implementation of all aspects of the IIIF Authorization Flow specification.
- [iiif-image-auth](https://github.com/robcast/iiif-image-auth) - (IIIF Auth 1.0) A simple server implementation based on Docker and Flask.
- [IIIF.io : the hardest part will be saying "no".](http://mcormond.blogspot.com/2017/06/iiif-hardest-part-saying-no.html) - Blog post by Russell McOrmond considering the challenges of restricting access to Canadiana's resources.

## Tutorials

Tutorials for how to accomplish functionality in your applications.

- [IIIF Online Workshop](https://training.iiif.io/iiif-online-workshop/) - IIIF workshop materials and videos given by the IIIF-C and updated at each occurrence.
- [Archiviiify](https://literarymachin.es/archiviiify/) - A short guide to download digitized books from Internet Archive and rehost on your own infrastructure using IIIF with full-text search [from raffaele messuti / [@atomotic](https://github.com/atomotic)].
- [Drag and Drop](https://medium.com/@aeschylus/create-and-share-iiif-items-quickly-and-easily-with-drag-and-drop-over-email-879f13c9caba) - Getting a IIIF image into Mirador with drag-and-drop and email.
- [Experiments with IIIF and Gallica](https://github.com/altomator/IIIF/) - A guided tour of end user applications of IIIF to Gallica materials, by Jean-Philippe Moreux (BnF).
- [Fellow Travelers: The Canterbury Tales and IIIF](https://blalbrit.github.io/2015/07/14/fellow-travelers-the-canterbury-tales-and-iiif) - Benjamin Albritton; includes an explanation of the use case for medieval scholars using Chaucer as an example and short section on how to make a page comparison demo in Mirador.
- [Introduction to APIs using IIIF](http://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/) - Uses IIIF as an example to explain APIs.
- [IIIF Implementation Guide](https://guides.iiif.io/guide_for_implementers/) - A step-by-step walkthrough of how to implement IIIF.
- [IIIF Intro (fr)](https://doc.biblissima.fr/introduction-iiif) - Introduction to IIIF (in French).
- [IIIF Workshop for DHNord2020](https://github.com/regisrob/Atelier_IIIF_Conference_DHNord_2020) - French langauge workshop with three exercises from a workshop entitled "Adopt and use IIIF standards for your digital image corpora," created by Régis Robineau (technical coordinator of Biblissima) and Johann Holland (TGIR Huma-Num).
- [Image API Playground](https://www.learniiif.org/image-api/playground) - Learn about the structure of a IIIF URL through manipulating the parameters and seeing the results in a live demo.
- [Image Choice video](https://www.youtube.com/watch?v=4AJPVktQ1Zw) - Demonstration of how a canvas can have a choice of images and a viewer can toggle between them.
- [Introduction to APIs using IIIF](http://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/) - Uses IIIF as an example to explain APIs.
- [Introduction to IIIF](https://resources.digirati.com/iiif/an-introduction-to-iiif/) - A thorough introduction to the IIIF specifications and tools for using them, by Tom Crane at Digirati.
- [Introduction to IIIF in Portuguese](https://medium.com/ecologiadigital/conhecendo-o-iiif-padr%C3%B5es-e-ferramentas-para-publica%C3%A7%C3%A3o-de-imagens-na-web-a62af62a1b36) - Covers Image API, Presentation API, and annotations.
- [Suggested measures for deploying IIIF in Swiss cultural heritage institutions (White paper)](https://doi.org/10.5281/zenodo.2640415) - Julien A. Raemy & René Schneider (2019).

## Videos and Slide Decks

Slide decks and presentation videos with a focus on IIIF.

**For the most recent videos of lightning talks, papers, and semi-annual conference presentations, see the official [IIIF Consortium YouTube channel](https://www.youtube.com/iiif-consortium).**

- [An Introduction to the International Image Interoperability Framework](https://drive.google.com/file/d/0BwIq5pa1_rvfMnhCZmtzNTc5dnc/view) - Presentation introducing IIIF for new audiences as "the API for humans" - also contains videos from other IIIF presentations.
- [Collection of slide decks](http://www.slideshare.net/IIIF_io/clipboards) - From various IIIF events.
- [DHtech Workshop: Image Servers and IIIF](https://doi.org/10.20375/0000-000b-cb01-f) - Slides and recording from a DARIAH-DE workshop in 2018 by Robert Casties.
- [Image API Introduction](https://docs.google.com/presentation/d/1urCPiL3LffkIWglKGW4SSEiojBt2_RKmt5YuDtBoRfY/edit?usp=sharing) - High level overview of the Image API parameters.
- [IIIF For Small Projects](http://www.slideshare.net/workergnome/iiif-for-small-projects) - How IIIF can be used on small projects with limited infrastructure, presented at [KeystoneDH 2016](http://keystonedh.network/2016/).
- [IIIF Tutorials (German)](https://www.youtube.com/playlist?list=PLxDekeBVQtVJeRqoTgsif7fJki2X96O-1) - YouTube playlist from the Zurich Central Library (Zentralbibliothek Zürich).
- [Introduction to the Presentation API](http://www.slideshare.net/azaroth42/iiif-presentation-api) - Rob Sanderson.
- [OA - Shared Canvas - TEI - Biblissima project](http://www.slideshare.net/biblissima/oa-shared-canvas-tei-biblissima-project) - Part of a workshop on TEI and neighboring standards including IIIF.
- [Video from IIIF event at the National Gallery of Art](https://www.youtube.com/playlist?list=PLYPP1-8uH9c6iQpKTXnhnlQpmoMLT1fB7) - May 2015.
- [Video from the outreach event at the Museum of Modern Art ](https://www.youtube.com/playlist?list=PLYPP1-8uH9c5smSD2wyVgsqKxD218khZq) - May 2016.



## Discovery

Links to help you discover IIIF resources that have been shared, demonstrations of IIIF discovery and useful discovery tools.

- [Biblissima IIIF-Collections](https://iiif.biblissima.fr/collections/) - Prototype application that allows you to search across IIIF-compliant manuscripts and rare books dated before 1800.
- [Cultural Japan](https://cultural.jp/) - Discovery system for IIIF resources in Japan.
- [detektIIIF2](https://chrome.google.com/webstore/detail/detektiiif2/aaodcobgcadinjipaocibamdfcffpcpp) - a Chrome extension that automatically detects IIIF resources in web pages and offers users a convenient way to collect and reuse them. 
- [Europeana's IIIF filtered search](https://www.europeana.eu/portal/en/search?q=provider_aggregation_edm_isShownBy%3A*iiif*&view=grid) - Europeana provides a filter to identify all IIIF-enabled resources in its collections.
- [iiif-universe](https://github.com/ryanfb/iiif-universe) - Repository that includes links to known IIIF presentation manifest collections.
- [iNQUIRE demo](http://inquire.armtest.uk/) - Open-source IIIF-compliant research and discovery platform. This is the IIIF-compliant version of the platform driving [Digital Bodleian] (http://digital.bodleian.ox.ac.uk/).
- [iNQUIRE source](https://github.com/armadillo-systems/inquire) - Github repository for iNQUIRE.
- [museum-digital](https://global.museum-digital.org) - Portal that provides access to digital objects from many museums (mostly in Germany and Central Europe), some of which are IIIF-enabled.

### Import to Viewers

- [iiif.link](https://github.com/atomotic/iiif.link) - A url shortener for sharing a IIIF resource; upon opening the URL the viewer will open at the saved zoom and region of interest.
- [Open in IIIF Viewer](https://github.com/2SC1815J/open-in-iiif-viewer) - A web browser extension to open IIIF manifest link in your favorite IIIF viewer. 
- 

## Annotations

- [ALTO to Annotation list](https://github.com/glenrobson/iiif_stuff/tree/master/alto2annotations) - This XSLT converts an ALTO xml document to an annotation lists for use with a IIIF manifests.
- [Annocoda](https://github.com/jptmoore/annocoda) - Mobile-friendly web app that uses IIIF Content Search 2.0 and Presentation 3.0 to provide image search capabilities
- [Annona Annotation Library: iiif-annotation viewer JavaScript library](https://ncsu-libraries.github.io/annona/) - JavaScript library that uses custom tags and url of the annotation to load annotated image, corresponding annotations, tags, and text into HTML object or OpenSeadragon viewer with overlays.
- [Glycerine Workbench](https://glycerine.io/) – A scholarly annotation and publication workbench.   Glycerine provides end-to-end workflows for collaboration and publishing of images.  Glycerine is a comprehensive framework for institutional integration.
- [Recogito](https://recogito.pelagios.org/) - A popular and award-winning Digital Humanities platform for collaborative document annotation, maintained by [Pelagios](https://pelagios.org/). 
- [Storiiies](http://storiiies.cogapp.com/) - Demos of using annotations for storytelling.

### Annotation Servers

- [annotot](https://github.com/PenguinParadigm/annotot) - Simple IIIF annotations mounted in a Ruby on Rails applications.
- [CatchPy](https://github.com/nmaekawa/catchpy) - Django-based annotation server with support for Web Annotation and AnnotatorJS APIs, using JWT for auth. Originally developed for the AnnotationsX LTI tool, CatchPy also supports tagging and responses.
- [Elucidate](https://github.com/dlcs/elucidate-server) - Java and Postgres annotation server.
- [Europeana](https://github.com/europeana/annotation) - Extension to the Europeana REST API that allows you to create, retrieve, and manage annotations on Europeana objects
- [ipfs-iiif-db](https://github.com/pgte/ipfs-iiif-db)[deprecated] - IIIF annotations JS client over IPFS.
- [Local IIIF Annotation Server](https://github.com/dnoneill/annotate)[deprecated] - Jekyll front end, Flask backend, equipped with Vagrant Box that provides a Mirador viewer for creating and save annotations into Jekyll site. Annotations are sharable by using GitHub pages with Jekyll front end.
- [MangoServer](https://github.com/azaroth42/MangoServer)[deprecated] - Mongo-backed annotation server written in Python.
- [Miiify](https://github.com/nationalarchives/miiify) - Light-weight annotation server built on the same principles as Git.
- [SimpleAnnotationServer](https://github.com/glenrobson/SimpleAnnotationServer) - Java annotation server backed by an Apache Jena triple store, Sesame, or Solr.

### Annotation Clients

- [Adno](https://adno.app/en/) - a web application for viewing, editing and sharing narratives and pathways on IIIF images.
- [Annonatate](https://annonatate.fly.dev/) - Website that allows users to create annotations via their GitHub account. The website saves all the annotations to the user's GitHub. Also makes use of Annona and allows users to create custom Annona views.
- [IIIF Annotation Studio](https://github.com/atomotic/iiif-annotation-studio) - Mirador Viewer packaged as a desktop app (macos, linux) with an embedded annotation endpoint that saves annotations to a local sqlite database.


## Crowdsourcing

- [Cratylus](https://apps.bowdoin.edu/cratylus/) - a crowd-sourced art tagging toolset.
- [iiif-annotations](https://github.com/zooniverse/iiif-annotations) - A proof-of-concept, annotating a IIIF manifest with Zooniverse classification data. See also [Importing images into Zooniverse with a IIIF manifest: introducing an experimental feature](https://blogs.bl.uk/digital-scholarship/2022/04/importing-images-into-zooniverse-with-a-iiif-manifest-introducing-an-experimental-feature.html) and [Fun with IIIF](https://blog.zooniverse.org/2022/04/20/fun-with-iiif/) on the ability to use IIIF to import media into the Zooniverse project builder.
- [FromThePage](https://fromthepage.com/) - a crowdsourcing platform for archives and libraries where volunteers transcribe, index, and describe historic documents.
- [Madoc](https://madoc.digirati.com/) - a flexible crowdsourcing, research and teaching platform for digitised collections.
- [Pybossa](https://pybossa.com/) - a crowdsourcing framework to analyze or enrich data that can't be processed by machines alone.
- [Recogito](https://recogito.pelagios.org/) - an online platform for collaborative document annotation.

## CMS Integration

Content Management Systems (CMS) modules that implement or leverage the IIIF APIs.

- [IIIF Image Field](https://www.drupal.org/sandbox/sdellis/2421047) - Drupal 7 module that provides an easy way to add IIIF Images to content types, and configure their display. Supports Image API versions 1.0 or 2.0.
- [IIIF Server Omeka S Module](https://omeka.org/s/modules/IiifServer/) - Omeka S module that implements the IIIF Image and Presentation APIs.
- [IIIF Toolkit](https://github.com/utlib/IiifItems) - IIIF Toolkit by University of Toronto Libraries is a plugin for Omeka Classic (2.3+) that integrates Mirador with a built-in annotator, a manifest generator, Simple Pages shortcodes and Exhibit Builder blocks for a rich presentation experience.
- [Inseri.com](inseri.core) - WordPress plugin with a IIIF Viewer block.
- [Mirador Viewer Omeka S Module](https://github.com/Daniel-KM/Omeka-S-module-Mirador) - Omeka S module that integrates the Mirador image viewer.
- [UniversalViewer Omeka S Module](https://omeka.org/s/modules/UniversalViewer/) - Omeka S module that integrates UniversalViewer.

## Wiki Integration

Wiki software tools that implement or leverage the IIIF APIs

- [Mirador extension to MediaWiki](https://github.com/a-g-van-hamel-foundation/Mirador) - MediaWiki extension which offers the Mirador Viewer along with a number of open-source plugins.

## Hosting

Internet file hosting that provides IIIF support (including both paid and free options). 

- [Digirati DLCS](https://iiif-cloud.digirati.com/)
- [Internet Archive](https://archive.org/)
- [Klokan](http://iiifhosting.com/) 
- [Micrio](https://micr.io/iiif)
- [iiif.fr](https://iiif.fr/) from Teklia

## Newspapers

These are resources that are specifically useful for working with newspapers. Many of them are outputs of the [IIIF Newspaper Community Group](http://iiif.io/community/groups/newspapers/) (now on hiatus).

- [Open ONI (Open Online Newspaper Initiative)](https://github.com/open-oni/open-oni) - Open Online Newspaper Initiative (Open ONI) is a community-maintained project to make historic American newspapers browsable and searchable on the web.
- [IIIF Newspapers Google Drive Folder](https://goo.gl/jNFfVw) - Working documents of the Interest Group for meeting minutes, and working drafts of best practices, etc.
- [ndnp_iiif](https://github.com/umd-mith/ndnp_iiif) - Python program for turning [National Digital Newspaper Program data](https://www.loc.gov/ndnp/) into static IIIF JSON that is ready for mounting on the Web.
- [Populating the Annotation Store with IIIF Annotation List](https://github.com/glenrobson/SimpleAnnotationServer/blob/master/doc/PopulatingAnnotations.md) - Provides instructions on how to edit OCR text using annotations in Mirador.
- [Welsh Newspapers Online](http://newspapers.library.wales/) - Provides access to over 1 million newspaper pages using the IIIF Image API.
- National Library of Wales' guide to [IIIF Newspapers](http://dev.llgc.org.uk/wiki/index.php?title=IIIF_Newspapers) provides an explanation and examples of how IIIF applies to newspapers.

## STEM

Science, Technology, Engineering, Math/Medicine

- [CellXplorer](https://courses.edx.org/courses/course-v1:HarvardX+MCB64.1x+2T2023/d16e07a5cec442eeb7cd9dfcb695dce0/)
Cell biology annotations in a deep zoom viewer
- [MicroDraw](https://microdraw.pasteur.fr/) - a web application to visualise and annotate collaboratively high resolution histology data. 

## Experiments and Fun

- [3D trade cards explorer](http://labs.cogapp.com/tc/) - A 3D environment that displays nineteenth-century trade cards from the [Boston Public Library](https://www.digitalcommonwealth.org/collections/commonwealth:gq67jz045). Designed to be viewed on a mobile phone, ideally with Google Cardboard. Created using three.js by Jon White, Cogapp.
- [Animal Crossing Art Generator](https://experiments.getty.edu/ac-art-generator) - Getty's tool leverages IIIF to create custom patterns featuring artwork from famous art collections around the world.
- [ANTLITZ.NINJA](https://antlitz.ninja) - Award-winning digital art app that cuts and re-combines historical portraits. Based on IIIF.
- [Atlascope](https://www.leventhalmap.org/articles/atlascope-explained-looking-between-the-cracks/) - a tool for exploring historic urban atlases in metropolitan Boston and telling stories about how places have changed over time. 
- [cover.boutique](https://cover.boutique) - Award-winning web application to create designs for smartphone cases from IIIF resources.
- [David Rumsey MapTab](https://chrome.google.com/webstore/detail/david-rumsey-map-collecti/fnheacjohhlddiffbmafmpoblbkfgmde?hl=en) - A IIIF powered, Chrome extension that displays a random map from the David Rumsey Map Collection everytime you open a new tab in your browser. Built using Leaflet-IIIF and React.js. Created by Jack Reed, Stanford University Libraries.
- [Fractals](http://www.appliediiif.org.uk/live/fractalshome.htm) - Deep zoom into a huge (1bn x 1bn pixel) fractal image, created by Sean Martin, Applied IIIF.
- [Wallpaper HDR](https://christianmahnke.de/en/post/hdr-iiif/) - Deep zoom of an HDR Image of an 70ies wallpaper - works in Chome-based browsers, with an HDR-capable monitor.
- [Haptic Feedback for a page from a fabric sample book using IIIF](https://christianmahnke.de/en/post/haptic-feedback/)
- [IIIF for Dolls](https://iiif-for-dolls.davidnewbury.com/) - use IIIF to create printable versions of your favorite work at a variety of scales.
- [IIIF Stereographs](https://stereograph.davidnewbury.com/) - Exploring Stereo Photos with IIIF
- [Image Comparison with a Magnifying Glass](http://resources.digirati.com/iiif/an-introduction-to-iiif/dee-mag.html) - Image comparison using leaflet magnifying glass by Digirati.
- [Image Comparison with a Slider](http://resources.digirati.com/iiif/an-introduction-to-iiif/dee-sbs.html) - Image comparison using leaflet slider by Digirati.
- [Moviemaps](https://www.leventhalmap.org/articles/roll-the-tape-with-moviemaps/) - a way to pair a video discussion with digital collections objects that zoom and pan while synchronized with the video, while still allowing free exploration.
- [Mouse-over animation](https://xn--blaufusstlpel-qmb.de/) - Animated IIIF images on mouse over, look at the hero section, drag to right to reveal more animations.
- [Old Map Room](https://itunes.apple.com/us/app/old-map-room/id1347431506) - An AppleTV application that uses IIIF to turn any room into a map room.
- [Puzzles! Powered by IIIF](http://puzzle.mikeapps.me/) - Drag-and-drop image tile puzzles created by Michael Appleby, Yale Center for British Art.
- [Sleep Stories](https://wellcometrust.github.io/annotation-viewer/quilt/) - Experiment with the W3C Web Annotation Data Model. The  annotations present a sequence of stories associated with a large image. Optimised for mobile. Created by Andrew Dyton and Stephen Fraser, Digirati, for Wellcome Collection.
- [Medieval Word Maker](http://blalbrit.github.io/iiif_make_words.html) - a Medieval Word Maker, created by Ben Albritton, Stanford University Libraries.
- [Storiiies](http://storiiies.cogapp.com/) - Cogapp's showcase of recent experiments in digital storytelling using IIIF.

## Community

IIIF is a community-based initiative that relies on active participation, discussion, and input. To get involved and learn more, see the [IIIF Community page](http://iiif.io/community/).

- Join the [IIIF-Discuss email list](https://groups.google.com/forum/#!forum/iiif-discuss).
- Join [IIIF Slack](https://docs.google.com/forms/d/e/1FAIpQLSdGV9QSFo8i2z1R5iIMP7B2JVhS9akHqcykWF5_y4mtWqVrBA/viewform) for the most up to date and broad discussions.
- Read the [IIIF Community Newsletters](https://iiif.io/newsletter/) to stay up to date with the latest community activities.
- [Submit a IIIF-related news item](https://goo.gl/forms/2LMe9zUHVBEbI62C3) to the IIIF Community Newsletter.
- Contribute to one of the [IIIF community and/or technical groups](http://iiif.io/community/groups/).
- Participate in the IIIF community calls. See the [IIIF community calendar](http://iiif.io/community/groups/) for details.
- Learn more about the [IIIF Consortium](http://iiif.io/community/consortium/).
- Attend a [IIIF event](https://iiif.io/news-and-events/).
- [iiif_io on Twitter](https://twitter.com/iiif_io).
- [IIIF on Mastodon](https://glammr.us/@IIIF).

## Collection Management Systems (CMSs) and Digital Asset Management (DAMs) that support IIIF

 - [Archipelago](https://archipelago.nyc/)
 - [Axiell Collections](https://www.axiell.com/solutions/product/axiell-collections/)
 - [Aviary](https://weareavp.aviaryplatform.com/)
 - [CollectiveAccess](https://collectiveaccess.org)
 - [ContentDM](https://www.oclc.org/en/contentdm/iiif.html)
 - [Goobi](https://goobi.io)
 - [Islandora](https://islandora.github.io/documentation/user-documentation/iiif/)
 - [Invenio](https://invenio-software.org/products/framework/) (Image API implementation via [invenio-iiif](https://github.com/inveniosoftware/invenio-iiif))
 - [Knowledge Integration CIIM](https://www.k-int.com/products/ciim/)
 - [Kitodo](https://www.kitodo.org/)
 - [Libnova/Libsafe](https://www.libnova.com/) (Image API)
 - [Luna](http://www.lunaimaging.com/iiif)
 - [Memorix Nexus](https://www.vitec-memorix.com/en/solutions/memorix-nexus/)
 - [Muzai.io platform](https://muzai.io) (based on [Brif](https://github.com/pierrz/brif))
 - [NetX](https://www.netx.net/)
 - [ResCarta](https://rescarta.org/)
 - [ResourceSpace](https://www.resourcespace.com/knowledge-base/api/iiif)
 - [Rosetta](https://knowledge.exlibrisgroup.com/Rosetta/Training/What's_New_Videos/Rosetta_5-3)

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, all contributors waive all copyright and related neighboring rights to this work.
