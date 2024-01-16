
<!-- README.md is generated from README.Rmd. Please edit that file -->

# A reproducible environment for the book An Introduction to Spatial Data Analysis and Statistics: A Course in R

<!-- badges: start -->
<!-- badges: end -->

This repository makes use of package
{[renv](https://rstudio.github.io/renv/)} to provide a reproducible
project environment to work with the book [An Introduction to Spatial
Data Analysis and Statistics: A Course in
R](https://paezha.github.io/spatial-analysis-r/).

The repository provides all the infrastructure to replicate the
environment used to create the book. This includes the version of `R` as
well as all packages used in the book.

## How to use this repository

1.  Install R (make sure to pick the correct operating system) - this is
    the programming language, it comes as a ‘core package’ here:
    <https://cran.rstudio.com/>

2.  Install RStudio (make sure to pick the correct operating system) -
    this is the an IDE here:
    <https://www.rstudio.com/products/rstudio/download/>.

3.  Download the Rtools43 installer (Windows) and run it to install:
    <https://cran.r-project.org/bin/windows/Rtools/rtools43/rtools.html>.
    If using a Mac this may be achieved through installing Xcode
    *untested*: <https://mac.r-project.org/tools/>

4.  Download the code as a .zip file from this repository:
    <https://github.com/paezha/Applied-Spatial-Statistics>. The
    repository contains a `renv.lock` file that specifies all the
    versions of the packages used in the webbook. Unzip the file and
    store it in an apprioriate directory. Use this folder to work on the
    course.

5.  Open up the `.RProj` file called “Applied-Spatial-Statistics”. This
    will be the `R` project you will work in all course. This will
    launch RStudio.

6.  Install your first `R` package “Renv”

<!-- -->

    install.packages("Renv")

7.  Close Rstudio. Restart your computer.

8.  Double click the Applied-Spatial-Statistics.Rproj file. This will
    relaunch RStudio. You will see a message in your console saying that
    your library is out of synch with the lock file. Let’s make sure
    they are both in sync by ‘restoring’ the state of your computer to
    match the versions specified in the .lock file. Run the following:

<!-- -->

    renv::restore()

If an individual library does not install, run:

    install.packages("XXXXX") #where the XXXXX are replaced with the package name
    #and then run again..
    renv::restore()

If this issue occurs again, repeat the above chunk.

9.  Restart `R` by going to Session -\> Restart R. Now click the “+”
    green button and open a new “R Markdown” file. Select the 4th option
    in the left panel “From Template”. Select a template option from the
    {isdas} package. Each template is 1 chapter/activity in the webook.
    Give the template a name, say “my-template-chapter-1”.

10. Knit the “my-template-chapter-1.Rmd” to a .pdf file by clicking the
    arrow on the “Knit” button and selecting “PDF”.

You’ve just knitted your first PDF file! Congrats.
