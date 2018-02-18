---
layout: page
title: Software
permalink: /Software/
---

<h1 class="page-title">{{ page.title | escape }}</h1>

#### Overview

The second half of the course will involve hands-on tutorials for methods in macroevolution. We will ensure that everyone has the necessary software installed before this part of the course begins. 

#### Required Software

<div class="divider"></div>

##### Text editor

Everyone should have a good text editor. Here are some that we recommend:

* [Sublime Text](https://www.sublimetext.com/) (Linux, Windows, Mac OSX)
* [Atom](https://atom.io) (Linux, Windows, Mac OSX)
* [BBEdit](https://www.barebones.com/products/bbedit/) (Mac OSX)
* [Notepad++](https://notepad-plus-plus.org/) (Windows)
* Of course Vim/vi or Emacs are great (if that is your thing)

<div class="divider"></div>


##### RevBayes

RevBayes is a program for Bayesian phylogenetic inference. You can download compiled binaries for Mac OSX and Windows here: [http://revbayes.github.io/software.html](http://revbayes.github.io/software.html). If you have the Linux operating system, please follow the instructions for compiling the program from source.

For Bayesian phylogenetic inference, it is also useful to have the program Tracer for visualizing MCMC samples of numerical parameters. You can download Tracer here: [http://tree.bio.ed.ac.uk/software/tracer/](http://tree.bio.ed.ac.uk/software/tracer/).

<div class="divider"></div>

##### R

Install R and the suite of comparative phylogenetic methods packages.

* Download and R for your operating system: [https://cran.r-project.org](https://cran.r-project.org/)
* We recommend using **RStudio** [https://www.rstudio.com](https://www.rstudio.com/) as your interactive development environment for `R`.

Once you have R installed and you can open the R terminal, you can install several packages needed for performing comparative phylogenetic analyses. We will do this using the CRAN [phylogenetics task view](https://cran.r-project.org/web/views/Phylogenetics.html) that was created by [Brian O'Meara](http://brianomeara.info/). To do this, open R and execute the following lines:

```
install.packages("ctv")
library("ctv”)
install.views("Phylogenetics”)
```

It is possible that there are dependencies that you may have to install before you can successfully execute the task view. (We can troubleshoot these issues in class.)

The CRAN phylogenetics task view uses the release version of the `geomorph` pacakge. For our class, we will be using some more advanced methods in this package. So we will install the development version. To do this execute these lines in R:

```
install.packages("devtools")
devtools::install_github("geomorphR/geomorph",ref = "Develop")
```


<div class="divider"></div>

