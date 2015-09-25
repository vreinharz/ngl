
![Gallery](gallery.png)


NGL Viewer is a web application for molecular visualization. [WebGL](https://get.webgl.org/) is employed to display molecules like proteins and DNA/RNA with a variety of representations.


See it in action:

* [Web application](http://proteinformatics.charite.de/ngl)
* [Documentation](http://proteinformatics.charite.de/ngl/doc)


Features
========

* Molecular structures (mmCIF, PDB, GRO, SDF, MOL2)
* Density volumes (MRC/MAP/CCP4)
* User interaction (mouse picking, selection language, image export)
* Coordinate trajectories (animation, server)
* Embeddable (single file, API)


Acknowledgments
===============

This project would not be possible without recourse to many fine open-source projects. Especially the [three.js](http://threejs.org/) project provides a great foundation. See [here](http://proteinformatics.charite.de/ngl/doc/index.html#User_manual/Development/Acknowledgment) for a detailed list of acknowledgments.


Changelog
=========

Version 0.6dev
--------------

* CODE: clearer atomnames handling for fiber creation
* FIX: residues at the end of fibers may not require all backbone atoms
* ADD: User-defined color schemes (API)
* CODE: Color handling code refactored exposing more parameters
* FIX: #7
* DOC: pull request instruction for developers
* Higher color contrast for GUI and documentation pages
* CODE: Basic support for async creation of representations (so far used for molecular surfaces and volume triangulation)
* WIP: scripting API
* CODE: chunked data loading and parsing via streamer class
* MIGRATION: Stage.loadFile signature changed
* CODE: faster autobonding of large residues (e.g. hydrated lipids)
* CODE: WebWorker support while using development and build files
* CODE: WebWorker used for decompression, parsing and surface generation
* ADD: Support for MOL2 and SDF files


Version 0.5
-----------

The first release.


License
=======

Generally MIT licensed, see the LICENSE file for details.
