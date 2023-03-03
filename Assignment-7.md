Untitled
================

### Package title

Simple Features for R

### Location

- <https://r-spatial.github.io/sf/>
- <https://cran.r-project.org/package=sfc>

### Vignettes

In addition to standard helpfiles, SF includes 7 formal vignettes
covering:  
1. Introduction to simple features (SF) for R  
2. Reading, writing, and converting SF  
3. Manipulating SF geometries  
4. Manipulating SF  
5. Plotting SF  
6. Miscellaneous  
7. Spherical geometry in SF using s2geometry

### Applications

1.  Example of [presentation](https://edzer.github.io/rstudio_conf/#1)
    on Tidy spatial data analysis.  
2.  A [published article](https://peerj.com/articles/11031.pdf) using sf
    to look at home-range estimation.  
3.  A [bookdown from
    UCSB](https://learning.nceas.ucsb.edu/2019-11-RRCourse/spatial-vector-analysis-using-sf.html)
    including a chapter on spatial vector analysis using SF.  
4.  A [blog post](https://hansenjohnson.org/post/animate-movement-in-r/)
    on animating telemetry data in SF format with gganimate.  
5.  A [tutorial on a
    blog](https://www.robwiederstein.org/2022/03/28/simple-features-tutorial-in-r-number-2/)
    about getting starting with sf.  
6.  A [github repo](https://github.com/ryangarnett/rSpatial) containing
    sf cheatsheets.

### Review

SF provides a standardized way of representing spatial data. SF for R
implements these practices into an R package. It allows you to create
“features” with some sort of associated spatial properties
(e.g. location or extent) following international standards.

I enjoy how well the package is integrated with Tidy. SF’s spiritual
predecessor, sp, was written prior to the development of the
aforementioned standards and prior to the widespread proliferation of
the tidyverse. Prior to sf there was no clear standardized way to work
with spatial data in R, and no easy way of working with these spatial sp
objects using Tidy practices. The spatial data structures in sf are
intended to integrate with the tidyverse and were built using its
guiding principles.

Because sf is a modern alternative to sp, there is some (in my opinion)
clunkiness in maintaining backwards compatibility with sp. Many of the
built-in functions have very-slightly-different names to try to help sp
users learn sf but then behave differently. I also have had to use both
sp and sf to accomplish things, especially when working with rasters and
time series data from monitoring stations (e.g. camera traps). Not all
packages have been migrated to work with sf and it can be confusing to
include both sp and sf in your workflow with all of the similarities in
function names and behavior.

I highly recommend this package and think if you have a novice grasp on
R, Tidy, and GIS you should be able to pick it up quickly! It’s a lot
more fun working with spatial data in R than faffing around in QGis or
Arc for ages.
