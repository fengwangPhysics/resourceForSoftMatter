# resourceForSoftMatter

online resource for soft matter (colloid) research

## particle tracking
* [trackpy](https://github.com/ronojoy/trackpy)
provides a mature version of `python` particle tracking implementation of the famous `IDL` tracking code from John Crocker and David Grier (www.physics.emory.edu/~weeks/idl/). Furthermore, it implements a few more advanced trackers to handle complicated situations.
* Particle Identification and Tracking: Particle Identification and Tracking (tacaswell.github.io/tracking/html/)
This is an implementation in `c++` of the particle tracking algorithms developed by Croker and Grier.

* `Matlab` Particle Tracking (site.physics.georgetown.edu/matlab/)

* [circletracking](https://github.com/caspervdw/circletracking): `python` tookits for tracking circles and ellipses in 2D or 3D images

* [EllipsoidFit](https://github.com/harukihirasawa/EllipsoidFit) can handle 3D ellipsoid

* [Rectangle_fit](https://github.com/harukihirasawa/Rectangle_fit) can handle rod

* [TubeTK](https://github.com/KitwareMedical/TubeTK) is an open-source toolkit for the segmentation, registration, and analysis of tubes and surfaces in images, developed by Kitware, Inc.

* [MathieuLeocmach/colloids](https://github.com/MathieuLeocmach/colloids) is a `C++` and `python` library to process both experimental and simulation data of colloidal particles. The main features are particle tracking from confocal microscopy images and analysis of local structure and dynamics of particles (from simulations or experiments).

## movie/image
* [ffmpeg](https://ffmpeg.org/) for making movies, and converting movie to images. It is a cross-platform solution to record, convert and stream audio and video. It includes libavcodec - the leading audio/video codec library.

* html files can embed videos, so that one can use browser to show movie. Media formats supported by HTML (Browser compatibility) should be
  * Theora and Vorbis in Ogg
  * H.264 and MP3 in MP4
  * H.264 and AAC in MP4
  * WebM

* ImageMagick (www.imagemagick.org/): Convert, Edit, Or Compose Bitmap Images

* [Inkscape](https://www.inkscape.org/) is professional quality vector graphics software which runs on Linux, Mac OS X and Windows desktop computers. It can be used to extract and edit figures from scientific papers in PDF format. Its default format is SVG. To convert pdf figures to SVG, one can use `pdftocairo` which has been installed on most Linux computers:
```
$ pdftocairo -svg input.pdf
```
* [pims](https://github.com/soft-matter/pims): Python Image Sequence: Load video and sequential images in many formats with a simple, consistent interface.

## Big data visualization
* [Bokeh](https://github.com/bokeh/bokeh) is a `python` project which targets browser-based graphics, and recent releases are beginning to do big data in the browser the right way. 
* [VisPy](https://github.com/vispy/vispy) is another effort to provide easy visualization of large datasets with `python`. It is based on `OpenGL`, with plans to add a `WebGL` backend.
* [mpld3](https://github.com/mpld3/mpld3) brings together `Matplotlib`, the popular `Python`-based graphing library, and `D3js`, the popular Javascript library for creating interactive data,  which can output SVG files. The library may require a little knowledge on javascript to enable flexible functions. It provides an interactive way to data visualization, rather than aiming on big data. d3.js gallery: https://github.com/d3/d3/wiki/Gallery. An example can be found: Visualizing MBTA Data: http://mbtaviz.github.io/

## Crystal defect identification
* [BiDef](https://github.com/mskarlin/BiDef]) is a python package using supervised machine learning for crystal defect identification. See details in the author's paper. It also seems that the package has something to do with `ovito`.
* [Atoman](https://github.com/chrisdjscott/Atoman) provides a python wrapper (written by C extension) on voro++, and algorithms to detect point defects by voronoi.

## Thesis
* W.L. Miller's thesis (https://github.com/wlmiller/thesis): Janus particles and aspherical particles MD simulation
* This thesis (https://github.com/jeffschulte/dissertation/blob/master/general_notes.tex) gives a note on FMT of hard spheres.

## Online learning materials
* [SklogWiki](http://www.sklogwiki.org/SklogWiki/index.php/Main_Page) is an open-edit encyclopedia dedicated to thermodynamics and statistical mechanics, especially that of simple liquids, complex fluids, and soft condensed matter.
