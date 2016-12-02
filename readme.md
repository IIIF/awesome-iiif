# Awesome IIIF [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A list of lists of awesome [IIIF](http://iiif.io/) resources.

The International Image Interoperability Framework (IIIF) is a group of standard APIs around sharing and reuse of media. It is also a growing community of galleries, libraries, archives, museums, companies, and others who develop the standards and interoperable software implementations. Content includes helpful links around each of the standards, demonstrations of their use, and tutorials and presentations. The list is especially helpful for orienting new community members and developers.

[![Contributing Guidelines](http://img.shields.io/badge/CONTRIBUTING-Guidelines-blue.svg)](./contributing.md)

**Disclaimer**: This list is created for informational purposes only and any links do not constitute an endorsement, recommendation, or favoring by the IIIF Consortium.

## Contents
- [Standards](#standards)
- [Image Servers](#image-servers)
- [Image Server Shims](#image-server-shims)
- [Image Viewers](#image-viewers)
- [Image API Libraries](#image-api-libraries)
- [Presentation API Libraries](#presentation-api-libraries)
- [Presentation API Shims](#presentation-api-shims)
- [Content Search API Servers](#content-search-api)
- [Tutorials](#tutorials)
- [Presentations and Slide Decks](#presentations-and-slide-decks)
- [Discovery](#discovery)
- [Implementations](#implementations)
- [Newspapers](#newspapers)
- [Writing](#writing)
- [Experiments and Fun](#experiments-and-fun)

## Standards

IIIF has developed several standards.

- [Image API](http://iiif.io/api/image/)
- [Presentation API](http://iiif.io/api/presentation/)
- [Content Search API](http://iiif.io/api/search/)
- [Authentication API](http://iiif.io/api/auth/)
- [External Services API Annex](http://iiif.io/api/annex/services/)

## Image Servers

These servers support the IIIF Image API. Some may also have support for the Presentation API.

- [Loris](https://github.com/loris-imageserver/loris) written in Python.
- [IIPImage Server](http://iipimage.sourceforge.net/documentation/server/) high performance image server.
- [riiif](https://github.com/curationexperts/riiif) written in Ruby as a Rails engine.
- [SIPI](https://github.com/dhlab-basel/Sipi) IIIFv2 image server written in C++.
- [RAIS](https://github.com/uoregon-libraries/rais-image-server) 100% open source tile server for JP2 images written in Go.
- [digilib](http://digilib.sourceforge.net) image server written in Java.
- [Cantaloupe](https://github.com/medusa-project/cantaloupe) image server written in Java.
- [iiif_s3](https://github.com/cmoa/iiif_s3) Ruby library for generating a static IIIF level 0 Image and Presentation API server on Amazon S3.
- [Hymir IIIF Server](https://github.com/dbmdz/iiif-server-hymir) IIIF server written in Java supporting IIIF Image and Presentation API.
- [go-iiif](https://github.com/thisisaaronland/go-iiif) IIIF server written in go (fork of [greut/iiif](https://github.com/greut/iiif)).

## Image Server Shims

These shims allow you to use an image server that does not currently support IIIF. If you have not implemented an image server yet, this is probably not where you want to start.

- [Djatoka Ruby gem](https://github.com/jronallo/djatoka) convert IIIF URLs into the URLs that Djatoka requires.
- [Shimmy](https://github.com/mejackreed/shimmy) is a Ruby gem designed to help you build shims for the IIIF Presentation API.
- [ContentDM Image translator](https://github.com/azaroth42/pi3f/tree/master/shims/ContentDM) makes ContentDM images available through IIIF. Python.
- [Flask-IIIF](https://github.com/inveniosoftware/flask-iiif) Flask extension to support IIIF in Python/Flask applications. See [Flask-IIIF previewer demo](http://flask-iiif.herokuapp.com/previewer) and [Flask-IIIF RESTful demo](http://flask-iiif.herokuapp.com/restful).

## Image Viewers
- [Universal Viewer](https://github.com/UniversalViewer/universalviewer) is a rich embeddable interface.
- [OpenSeadragon](https://openseadragon.github.io/examples/tilesource-iiif/) has IIIF tile support.
  - [Scalebar Plugin](https://github.com/NIST-ISG/OpenSeadragonScalebar) OpenSeadragon plugin for physical scale overlay.
  - [Imaging Helper Plugin](https://github.com/msalsbery/OpenSeadragonImagingHelper) OpenSeadragon plugin with utility functions.
- [Leaflet-IIIF](https://github.com/mejackreed/Leaflet-IIIF) lightweight, extensible IIIF image viewer.
- [Mirador](https://github.com/IIIF/mirador) multi-up workspace.
- [Diva.js](https://ddmal.github.io/diva.js/) IIIF image viewer optimized for speed and flexibility.

## Image API Libraries
- [iiif-image-api](https://github.com/dbmdz/iiif-image-api) Java IIIF Image API libraries.
- [piffle](https://github.com/emory-lits-labs/piffle) Python library for generating and parsing IIIF Image API URLs.
- [iiif_url](https://github.com/NCSU-Libraries/iiif_url) Ruby library for creating and parsing IIIF Image API URLs.

## Presentation API Libraries
- [Manifesto](https://github.com/UniversalViewer/manifesto) IIIF Presentation API client and server utility library.
- [Manifold](https://github.com/UniversalViewer/manifold) Wraps Manifesto to provide viewer state and related utilities.
- [O'Sullivan](https://github.com/IIIF/osullivan) Ruby API for creating IIIF manifests.
- [iiif-prezi](https://github.com/IIIF/iiif-prezi) Python library providing a reference implementation.
- [iiif-presentation-api](https://github.com/dbmdz/iiif-presentation-api) Java IIIF Presentation API libraries.
- [tabula-rasa](https://www.npmjs.com/package/tabula-rasa) npm module for creating and manipulating IIIF manifests.
- [iiif-tree-component](https://github.com/edsilv/iiif-tree-component) IIIF tree menu sortable by date with multi-select capability.
- [Tripoli](https://ddmal.github.io/tripoli/) IIIF Presentation API 2.0+ validation library.

## Presentation API Shims

These shims allow you to use systems with presentation metadata (e.g. structure or sequences) that do not currently support IIIF. If you have not implemented the Presentation API yet, this is probably not where you want to start.

- [Shimmy](https://github.com/mejackreed/shimmy) is a Ruby gem designed to help you build shims for the IIIF Presentation API, and has samples for NYPL, Flickr, and the US National Archives.
- [Chronicling America](https://github.com/azaroth42/presentation-api-shims/tree/master/shims/chronam) for newspapers digitized in the National Digital Newspaper Program.

## Content Search API

Libraries and applications that support the Content Search API.

- [Ocracoke](https://github.com/NCSU-Libraries/ocracoke) - Rails application to create, index, and search text from page images and provide results in IIIF Content Search API format.

## Tutorials

Tutorials for how to accomplish functionality in your applications.

- [IIIF Image API live demo](http://yenda.tools/en/iiif-api-demo-en/) Learn about the structure of a IIIF URL through manipulating the parameters and seeing the results in a live demo.
- [IIIF Quick Start Guide](http://iiif.io/technical-details/) is a quick overview of how you might get started with implementing various IIIF standards.
- [Drag and Drop](https://medium.com/@aeschylus/create-and-share-iiif-items-quickly-and-easily-with-drag-and-drop-over-email-879f13c9caba) a IIIF image into Mirador.
- [Fellow Travelers: The Canterbury Tales and IIIF](http://web.stanford.edu/group/dmstech/cgi-bin/wordpress/author/blalbrit/) by Benjamin Albritton includes an explanation of the use case for medieval scholars using Chaucer as an example and short section on how to make a page comparison demo in Mirador.
- [IIIF Intro (fr)](http://doc.biblissima-condorcet.fr/introduction-iiif) Introduction to IIIF (in French).
- [Introduction to APIs using IIIF](http://www.meanboyfriend.com/overdue_ideas/2016/06/introduction-to-apis-using-iiif/) uses IIIF as an example to explain APIs.
- [Image Choice video](https://www.youtube.com/watch?v=4AJPVktQ1Zw) demonstration of how a canvas can have a choice of images and a viewer can toggle between them.

## Presentations and Slide Decks

Slide decks with a focus on IIIF.

- [Image API Introduction](https://docs.google.com/presentation/d/1urCPiL3LffkIWglKGW4SSEiojBt2_RKmt5YuDtBoRfY/edit?usp=sharing) a high level overview of the Image API parameters.
- [OA - Shared Canvas - TEI - Biblissima project](http://www.slideshare.net/biblissima/oa-shared-canvas-tei-biblissima-project) part of a workshop on TEI and neighboring standards including IIIF.
- [IIIF For Small Projects](http://www.slideshare.net/workergnome/iiif-for-small-projects) how IIIF can be used on small projects with limited infrastructure, presented at [KeystoneDH 2016](http://keystonedh.network/2016/).
- [Introduction to the Presentation API](http://www.slideshare.net/azaroth42/iiif-presentation-api) by Rob Sanderson.
- [Video from the outreach event at the Museum of Modern Art ](https://www.youtube.com/playlist?list=PLYPP1-8uH9c5smSD2wyVgsqKxD218khZq) in May 2016.
- [Collection of slide decks](http://www.slideshare.net/IIIF_io/clipboards) from various IIIF events.

## Discovery

Links to help you discover IIIF resources that have been shared, demonstrations of IIIF discovery and useful discovery tools.

- [iiif-universe](https://github.com/ryanfb/iiif-universe) is a repository that includes links to known IIIF presentation manifest collections.
- [iNQUIRE demo](http://inquire.armtest.uk/) is a demo of an open-source IIIF-compliant research and discovery platform. This is the IIIF-compliant version of the platform driving [Digital Bodleian] (http://digital.bodleian.ox.ac.uk/).
- [iNQUIRE source](https://github.com/armadillo-systems/inquire) is the Github repository for iNQUIRE.
- [Musiclibs](https://musiclibs.net) provides cross-library search of thousands of musical scores and manuscripts.

## Implementations

Sites which have implemented IIIF in some respect. Note what standards or other libraries are implemented.

- [Historical State Search](http://historicalstate.lib.ncsu.edu/search) displays images via a IIIF image server.
- [FromThePage](http://www.fromthepage.com) ingests IIIF manifests and displays images for transcription using OpenSeaDragon.
- [SAT Taishōzō Image DB](http://dzkimgs.l.u-tokyo.ac.jp/SATi/images.php?alang=en) by the SAT Daizōkyō Text Database Committee in the DH initiative, the University of Tokyo adopts the IIIF Image and Presentation APIs including over 4,000 annotations displayed on Mirador.
- [e-codices](http://www.e-codices.unifr.ch) provides access to 1,500 Swiss medieval manuscripts (ca. 500,000 high-res images) via IIIF. The IIIF manifest link for individual manuscripts can be found on the overview page of each manuscript (see [example](http://www.e-codices.unifr.ch/en/searchresult/list/one/csg/0857)). IIIF collection of collections with links to all manifests here: <http://www.e-codices.unifr.ch/metadata/iiif/collection.json>.
- [Gallica](http://gallica.bnf.fr/) is the digital library of the Bibliothèque nationale de France (BnF), providing access to millions of documents (newspapers and journals, maps, printed books, manuscripts, scores etc.). It implements the Image API and the Presentation API. [More technical details](http://doc.biblissima-condorcet.fr/entrepots-iiif-biblissima) about the IIIF endpoints (images and manifests).
- [Biblissima reconstituted manuscript demo](http://demos.biblissima-condorcet.fr/chateauroux/osd-demo/) presents a manuscript where illuminations had been cut out and then allows for reconstituting the manuscript by placing those images back into place.
- [iiif-server-demo](https://github.com/dbmdz/iiif-server-demo) Self-contained IIIF Demo server written in Java.
- [NCSU Libraries Rare and Unique Digital Collections](https://twitter.com/vaticanlibrary/status/732546207457935360) implements the Image, Presentation, and Content Search APIs.
- [DigiVatLib](http://digi.vatlib.it/) provides access to digitized collections from the Vatican.
- [Georeferencer](http://www.georeferencer.com/) can take maps accessible via IIIF and referenced to modern maps.
- [hocrviewer](https://github.com/jbaiter/hocrviewer-mirador) can display and search OCRed documents in the [hOCR format](http://kba.github.io/hocr-spec/1.2/) with Mirador. Contains a simple implementation of the Content Search API with SQLite.

## Newspapers

These are resources that are specifically useful for working with newspapers. Many of them are outputs of the IIIF Newspaper Interest Group.

- [IIIF Newspapers Google Drive Folder](https://goo.gl/jNFfVw) has working documents of the Interest Group for meeting minutes, and working drafts of best practices, etc.
- [Welsh Newspapers Online](http://newspapers.library.wales/) provides access to over 1 million newspaper pages using the IIIF Image API.
- [Populating the Annotation Store with IIIF Annotation List](https://github.com/glenrobson/SimpleAnnotationServer/blob/master/doc/PopulatingAnnotations.md) which provides instructions on how to edit OCR text using annotations in Mirador.
- [open-oni](https://github.com/open-oni/open-oni) is a friendly fork of [chronam](https://github.com/libraryofcongress/chronam) which is a webapp for viewing National Digital Newspaper Program data from the Library of Congress.
- [docker-open-oni](https://github.com/open-oni/docker-open-oni) is a Docker friendly setup for open-oni, which will set up and configure the Web application as well as the MySQL, Solr and RAIS Image Server.
- [ndnp_iiif](https://github.com/umd-mith/ndnp_iiif) is a Python program for turning [National Digital Newspaper Program data](https://www.loc.gov/ndnp/) into static IIIF JSON that is ready for mounting on the Web.

## Writing

Blog posts, press releases, and other writing about IIIF.

- [IIIF support for the Qatar Digital Library](http://www.cogapp.com/blog/iiif-support-qatar-digital-library).
- [Comprendre IIIF et l’interopérabilité des bibliothèques numériques](http://bsa.biblio.univ-lille3.fr/blog/2016/11/comprendre-iiif-interoperabilite-bibliotheques-numeriques/) blog post giving an overview of IIIF, in French.

## Experiments and Fun

- [Puzzles! Powered by IIIF](http://puzzle.mikeapps.me/) - Drag-and-drop image tile puzzles created by Michael Appleby, Yale Center for British Art.
- [Slider puzzles](http://blalbrit.github.io/puzzles) - More drag-and-drop puzzles, created by Ben Albritton, Stanford University Libraries.
- [David Rumsey MapTab](https://chrome.google.com/webstore/detail/david-rumsey-map-collecti/fnheacjohhlddiffbmafmpoblbkfgmde?hl=en) - A IIIF powered, Chrome extension that displays a random map from the David Rumsey Map Collection everytime you open a new tab in your browser. Built using Leaflet-IIIF and React.js. Created by Jack Reed, Stanford Univerity Libraries.
- [Fractals](http://showcase.iiif.io/showcase/fractals.html) - Deep zoom into a huge (1bn x 1bn pixel) fractal image, created by Sean Martin, Applied IIF. Also see [full list of fractals](http://www.appliediiif.org.uk/live/fractalshome.htm).
- [The Transcriptinator](http://labs.cogapp.com/transcriptinator/) - A prototype "game" created for use on the British Library's crowd-sourcing arcade machine. Players have to flag up errors in the OCR transcriptions of content taken from the [Qatar Digital Library](http://www.qdl.qa). Created by Jon White and Tristan Roddis, Cogapp.
- [IIIF Gallery](http://digirati-co-uk.github.io/iiif-gallery/src/) - A virtual art gallery using OpenSeadragon and custom image generation, created by Stephen Fraser, Digirati. Also see [full source code](https://github.com/digirati-co-uk/iiif-gallery/).
- [Exquisite Corpse](https://github.com/harvardartmuseums/exquisite-iiif-demo) - A prototype that deliberately mixes up portrait paintings. Created using Node.js by Jeff Steward, Harvard Art Museums.
- [3D trade cards explorer](http://labs.cogapp.com/tc/) - A 3D environment that displays nineteenth-century trade cards from the [Boston Public Library](https://www.digitalcommonwealth.org/collections/commonwealth:gq67jz045). Designed to be viewed on a mobile phone, ideally with Google Cardboard. Created using three.js by Jon White, Cogapp.

## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, all contributors waive all copyright and related neighboring rights to this work.
