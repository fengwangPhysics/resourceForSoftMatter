# resourceForSoftMatter

free online resource for soft matter (colloid) research

## Contents
* [particle tracking](#particle-tracking)
* [movie/image](#movieimage)
* [Big data visualization](#big-data-visualization)
* [Crystal defect identification](#crystal-defect-identification)
* [Thesis](#thesis)
* [Online learning materials](#online-learning-materials)
* [Latex and PDF files](#latex-and-pdf-files)
* [Useful data structures and algorithms](#useful-data-structures-and-algorithms)


## particle tracking
* [trackpy](https://github.com/ronojoy/trackpy)
provides a mature version of `python` particle tracking implementation of the famous `IDL` tracking code from John Crocker and David Grier (www.physics.emory.edu/~weeks/idl/). Furthermore, it implements a few more advanced trackers to handle complicated situations. However, it seems that it lacks an image noise filter.
* Particle Identification and Tracking: Particle Identification and Tracking (tacaswell.github.io/tracking/html/)
This is an implementation in `c++` of the particle tracking algorithms developed by Croker and Grier.

* `Matlab` Particle Tracking (site.physics.georgetown.edu/matlab/)

* [circletracking](https://github.com/caspervdw/circletracking): `python` tookits for tracking circles and ellipses in 2D or 3D images

* [EllipsoidFit](https://github.com/harukihirasawa/EllipsoidFit) can handle 3D ellipsoid

* [Rectangle_fit](https://github.com/harukihirasawa/Rectangle_fit) can handle rod

* [TubeTK](https://github.com/KitwareMedical/TubeTK) is an open-source toolkit for the segmentation, registration, and analysis of tubes and surfaces in images, developed by Kitware, Inc.

* [MathieuLeocmach/colloids](https://github.com/MathieuLeocmach/colloids) is a `C++` and `python` library to process both experimental and simulation data of colloidal particles. The main features are particle tracking from confocal microscopy images and analysis of local structure and dynamics of particles (from simulations or experiments).

## movie/image
* [ffmpeg](https://ffmpeg.org/) for making movies, and converting movie to images. It is a cross-platform solution to record, convert and stream audio and video. It includes libavcodec - the leading audio/video codec library. `h.264` encoder is not included in this library. Hence if h.264 is the desired format, it is necessary to install `x264` and compile `ffmpeg` with x264 enabled.
Here is an example to use `ffmpeg` (10 fps, bitrate: 1MB/s)
 ```
 $ ffmpeg -i figs/%04d.png -vcodec mpeg4 -r 10 -b:v 1M output.avi
 ```

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
* [pims](https://github.com/soft-matter/pims): Python Image Sequence: Load video and sequential images in many formats with a simple, consistent interface. It has the same authors as `trackpy`.

* [moviepy](https://github.com/Zulko/moviepy)
is a `Python` module for video editing.  It can read and write all the most common audio and video formats, including GIF, and runs on Windows/Mac/Linux

## Big data visualization
* [Bokeh](https://github.com/bokeh/bokeh) is a `python` project which targets browser-based graphics, and recent releases are beginning to do big data in the browser the right way. 
* [VisPy](https://github.com/vispy/vispy) is another effort to provide easy visualization of large datasets with `python`. It is based on `OpenGL`, with plans to add a `WebGL` backend.
* [mpld3](https://github.com/mpld3/mpld3) brings together `Matplotlib`, the popular `Python`-based graphing library, and `D3js`, the popular Javascript library for creating interactive data,  which can output SVG files. The library may require a little knowledge on javascript to enable flexible functions. It provides an interactive way to data visualization, rather than aiming on big data. d3.js gallery: https://github.com/d3/d3/wiki/Gallery. An example can be found: Visualizing MBTA Data: http://mbtaviz.github.io/

* [OVITO](http://ovito.org/) is a scientific visualization and analysis software for atomistic simulation data developed by Alexander Stukowski at Darmstadt University of Technology, Germany. It can be also used to visualize experimental data if the data is saved as the one of the following formats: LAMMPS, XYZ, IMD, CFG, POSCAR, AMBER/NetCDF, PDB, GSD/HOOMD, and VTK. See the description of those formats: http://ovito.org/manual/usage.import.html

* https://github.com/jbmouret/matplotlib_for_papers
uses `matplotlib` to plot statistical figures. Good example for box plot, Stars (statistical significance).

## Crystal defect identification
* [BiDef](https://github.com/mskarlin/BiDef]) is a python package using supervised machine learning for crystal defect identification. See details in the author's paper. It also seems that the package has something to do with `ovito`.
* [Atoman](https://github.com/chrisdjscott/Atoman) provides a python wrapper (written by C extension) on voro++, and algorithms to detect point defects by voronoi.

## Thesis
* W.L. Miller's thesis (https://github.com/wlmiller/thesis): Janus particles and aspherical particles MD simulation
* This thesis (https://github.com/jeffschulte/dissertation/blob/master/general_notes.tex) gives a note on FMT of hard spheres.

## Online learning materials
* [SklogWiki](http://www.sklogwiki.org/SklogWiki/index.php/Main_Page) is an open-edit encyclopedia dedicated to thermodynamics and statistical mechanics, especially that of simple liquids, complex fluids, and soft condensed matter.

## Latex and PDF files
* [Latex Wikibook](https://en.wikibooks.org/wiki/LaTeX) is a very good start point to learn latex.

* [Overleaf](https://www.overleaf.com/) is an online `LaTeX` and Rich Text collaborative writing and publishing tool that makes the whole process of writing, editing and publishing scientific documents much quicker and easier. 

* https://github.com/jdleesmiller/latex-course
An interactive introduction to `LaTeX` using [Overleaf](https://www.overleaf.com/).

* [Overleaf templates](https://www.overleaf.com/latex/templates/): Start your projects with quality LaTeX templates for journals, CVs, resumes, papers, presentations, assignments, letters, project reports, and more. 

* [zotero](https://github.com/zotero/zotero) is a free, easy-to-use tool to help you collect, organize, cite, and share your research sources. It is a useful reference manager which can export `bibtex`.

* https://github.com/citation-style-language/styles
Official repository for Citation Style Language (CSL) citation styles.

* merge PDF files:
 * `pdfunite` is a part of poppler, however, someone pointed out that the output.pdf may be very large while `gs` packs a small size.
 ```
$ pdfunite in1.pdf in2.pdf out.pdf
 ```
 * use `gs`
 ```
$ gs -dBATCH -dNOPAUSE -q -sDEVICE=pdfwrite -sOutputFile=out.pdf in1.pdf in2.pdf
 ```

## Useful data structures and algorithms
* https://github.com/jwasham/google-interview-university gives a lots of well-organized links and learn materials on commonly used data structure, as well as many other basic knowledges on programming.

* [k-d tree](https://en.wikipedia.org/wiki/K-d_tree) is a space-partitioning data structure for organizing points in a k-dimensional space. It is useful to obtain nearest neighbors with an O(log n) complexity. `scipy.spatial.KDTree` and `scipy.spatial.cKDTree` are two very fast implementations in python and C. (https://github.com/prody/ProDy/tree/master/prody/kdtree) has an implementation of kd-tree which can handle periodic boundary condition. A more general algorithm is `cover tree` which can handle any distance metric in arbitary high dimensional space. There are some C++ cover-tree implementations on github. The speed of the algorithm is very fast: one of implementations claimed that it takes 250 seconds for inserting 10^6 1000-dimensional vectors, and achieves 300 queries per second.

* [A gallery of interesting IPython Notebooks](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks)

* https://gist.github.com/nzjrs/990493 shows ways to interface python + C via ctypes or python module extensions.

* https://github.com/fengwangPhysics/ctypes-example is an example module to interface python + C via ctypes or python module extensions.
