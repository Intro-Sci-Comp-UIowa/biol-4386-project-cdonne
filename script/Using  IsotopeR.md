This markdown file is based on the  IsotopeR user guide found here, http://jackhopkinswildlife.com/isotoper/
#  IsotopeR 

IsotopeR is a is a mixture model designed for stable isotope analysis in R

### Installing IsotopeR

- Install JAGS for Mac http://sourceforge.net/projects/mcmc-jags/  
- Install JAGS for Windows http://sourceforge.net/projects/mcmc-jags/files/JAGS/4.x/Windows/
- Mac users with R before v3.0 must install tcltk software http://cran.r-project.org/bin/macosx/tools/and all mac users must also install XQuartz 2.7.8 http://www.xquartz.org/.  For smootheroperation, update your computer to R 3.2.2 for Mac OS X 10.9 or higher.
- Install ”IsotopeR” and the following dependencies (packages:fgui, runjags, ellipse, plotrix, colorspace) 
 
```sh
> install.packages("IsotopeR", dep=T)
```
### Running IsotopeR 
IsotopeR uses a Graphical User Interface (GUI)
```sh
> library(IsotopeR) # loads the package 
> IsotopeR() # opens the GUI 
```

###  Data files
- Mixtures (necessary file)
- Sources (necessary file)
- Concentrations (optional file)
- Discrimation error (optional file)
- Measurment error (optional file)


### Formatting Data files

To correctly format your data files, it is best to copy and paste your data into the example files found here, http://jackhopkinswildlife.com/isotoper/, and save. This will ensure that the data files will be formatted correctly for IsotopeR

### Input data files 
- From the GUI main menu click Anlysis --> New Run 
- In the data input screen, click on each of the left-hand button next to the apporpriate file to choose a file from your hard drive


### Parameters 
Control Parameters can be changed by the user. These are found below the file input section in the data input screen 
Each option can be turned on (TRUE) and off (FALSE)
 - Number  of  [Markov]  chains:   The  number  of  independent  Markov  chains  for  sampling  theparameter space and computing posterior quantities
 - MCMC burn-in: The length of the chain discarded at the beginning of the run, so that the effectof initial values on the posterior inference is minimized.  This is interpreted as the length of timeit takes for the MCMC to stabilize
 - MCMC runs:The total number of iterations per chain, excluding burn-in
 - Thinning rate:This feature reduces the sample size of each MCMC run by keeping everykthsimulated draw from each chain.  When thinning equals 1, the entire chain is saved
 - Plot observations:  Plots all raw isotope values for consumers and food items
- Plot mixing estimates:  Plots the estimated isotopic mixing space (the area contained in thespace formed by lines connecting sources in a multivariate plot).  The isotopic mixing space de-picts  the  mechanistic  relationship  between  consumers  and  their  foods  (i.e.,  the  environment  ofconsumers).  Sources are denoted by dashed ovals (2 SD)
- Plot dietary source contributions:  Plots the mean of the median posterior probability distri-bution for each major food source
- Run parallel: This boolean flag determines whether the MCMC chains should be run on separatecores of the processor (parallel=TRUE) or not (parallel=FALSE)


### Output files 
Parameter estimates will be automatically written to a text file (SampleOutput.txt) and an image file (SampleOutput.Rdata file), both located in the current working directory in R unless another output directory is defined by the user in the GUI. The .Rdata file name is specified in the field Output file

### Error messages 
Errors  are  often  associated  with  JAGS. Generally, these  errors  are  often  related  to  the  model  not  converging.   If  you  receive  an  error,  rerun  your analysis with more MCMC chains or use a higher thinning rate

### Using example data to test IsotopeR
- Download example data from http://jackhopkinswildlife.com/isotoper/
- Unzip the files 
- There are 2 data folders: 2-Isotope and 3-Isotope. For this project the 2-Isotope files was used
- Open IsotopeR in R
```sh
> library(IsotopeR) # loads the package 
> IsotopeR() # opens the GUI 
```
- Input each file from the 2-Isotope folder into the correct data file input 
- If the program was installed correctly then after running the model, plots will appear in R


