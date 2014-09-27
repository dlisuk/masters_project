masters_project
===============

This is a repository for my UCDS MS project.  I will keep a small journal of what I'm doing in this readme.

The goal of the project is to create an interactive data visualization framework within iPython to ease visual analysis of large data sets.  In particular I will connect the Pandas data frame to dc.js.

**September 19 2014**

  Today I got a scatter plot working using dc.js.  Additionally I hacked around with crossfilter/dc to figure out how to add a drop down menu which lets you choose a column to use for the x/y axis of the scatter plot. I also tried to work a static scatter plot into a ipython widget but it appears I still need to understand the widget interface quite a bit better.  It is based in jQuery so my next step is to learn jQuery sufficiently to debug the problems i'm seeing.

**September 18 2014**

  Today I learned about dc.js/crossfilter/d3.js.  Following tutorials from [codeproject](http://www.codeproject.com/Articles/693841/Making-Dashboards-with-Dc-js-Part-1-Using-Crossfil), I created a basic crossfilter data set feeding a dc/d3 visaul dash board.  Unlike our previous belief it turns out crossfilter is purely a client side data structure.  I believe that this is ok since it can be used to hold the data set locally for visaulization purposes.  
  
  Also I began looking into the widgit interface for ipython.  [This page](http://nbviewer.ipython.org/gist/rossant/9463955) contains a demo widgit for an editable pandas data frame which should serve as a useful starting point.  
  
  I created a ipython notebook based on the date widget from [this page](http://nbviewer.ipython.org/github/ipython/ipython/blob/2.x/examples/Interactive%20Widgets/Custom%20Widgets.ipynb).  It shows the basic code structure needed for a basic widget.