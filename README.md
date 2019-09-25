# intro to R workshop materials
This contains resources for RQDA lectures delivered on September, 2019, at JW LEE Center for Global Medicine. I would like to thank all the R community without which it won't be possible to compile these materials. 

This will Contains 
- R Code 
- Data for Practice 
- Presentation

# Software and Files

## R and RStudio Installation Instructions

This workshop assumes you have recent versions of R and RStudio. If you don't have R and RStudio Install from following links 

### For Windows 
R: https://cran.r-project.org/bin/windows/base/ 

R Studio: https://download1.rstudio.org/RStudio-1.1.463.exe

### For Mac
R: https://cran.r-project.org/bin/macosx/R-3.5.1.pkg

R Studio: https://download1.rstudio.org/RStudio-1.1.463.dmg

### For Linux (ubuntu)
R 
```ubuntu
# R with OpenBLAS
sudo apt-get install r-base
```
RStudio 

```ubuntu
# R with OpenBLAS
sudo apt-get install libopenblas-base r-base
```

## Workshop Materials

How to get the materials depends on how you plan to access R and RStudio for the workshop.

### On your laptop 

If you installed R and RStudio on your laptop, download all of the materials to your laptop.  Click on the green Clone or Download button above, then download the repository as a ZIP file.  

![github download](images/githubdownload.png)

Find the downloaded .zip file on your computer, likely in your Downloads folder.  Unzip it - usually by double-clicking.  This will create a directory.  Move this somewhere on your computer where you'll be able to find it, like your Documents folder.  

### using RStudio Cloud

If you're using RStudio Cloud, go to https://rstudio.cloud and log in (or create an account if needed).  Click on Your Workspace in the left Menu.  Then make sure you are on the Projects tab, and click down arrow in the blue button for New Project.  Choose the option of New Project from a Git Repo.  The repo address is https://github.com/prabinrs/intro_RQDA

![rstudio cloud new project](images/rstudiocloud.png)

This will copy all of the files from this repository into your new project.  This will take a few moments to copy files from this repository.  You'll then need to install packages.  Open `packagelist.r` and run the code.  The package will take a while to install and few of the features might not support be supported. For qualitative projects better not to use cloud version for now. 

You can use this space like you would your RStudio on own computer, except you can only access the files that are part of the project and save files within the project.

## Installing RQDA 
RQDA is R package for Qualitative Data Analysis. 
### for Windows 
**Step 1** Install GTK+, it can be downloded from http://downloads.sourceforge.net/gladewin32/gtk-2.10.11-win32-1.exe?modtime=1175123376&big_mirror=0 

** Step 2** Lunch R or R Studio from and install package RQDA 
```R
install.packages("RQDA", dependencies = c("Depends","Imports"))
```

**Step 3** Lunch and Test RQDA 
```R
library(RQDA) 
```
This should open RQDA GUI if doesn't open then 
```R
RQDA()
```

### for Linux
**Step 1** Install GTK+
```ubuntu
sudo apt-get install libgtk2.0-dev 
```
If this doesn't work, you might have to download manually and install. Please follow the instruction at https://developer.gnome.org/gtk3/stable/gtk-building.html

*follow step 2 and 3 as for the windows/base/

## for Mac OSX 
*if your system is yosemite and older then this won't work. Tested for OS X EI Capitan*
**Step 1** Install X11, download and install  XQuartz-2.7.7 from https://www.xquartz.org/

**Step 2** Install GTK+, download and install the binary package of GTK+ 2.24.17 from http://r.research.att.com/

*follow step 2 and 3 as for the windows


## Types of Files

**Slides:** The presentation fies are avaliable as Powerpoint.
 
**Dataset:**Transcribes of interviews as text file. The datasets are from the research project that explored the science and practice of ecological monitoring for adaptive management. The team conducted a qualitative case study of a project intended to develop an adaptive management approach to vegetation restoration in the ‘Wildlands National Park,’ Australia (hereafter referred to as 'the Wildlands AM project'). ‘Wildlands’ is a pseudonym – all place and personal names associated with the AM project have been changed to protect the participants’ anonymity. The data is avaliable for under CC0 "Public Domain Dedication" via Havard dataverse. 

## Other Resources
