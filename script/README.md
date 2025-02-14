# Markdown files 

- Using IsotopeR markdown file was added 4/15/20. This file contains the necessary information to help the user navigate IstotopeR
- IsotopeR parameters markdown file was added 4/23/20. This file contains the    paramenters used in the GUI(graphical user interface) of IsotopeR 
- IsotopeR.R script was added on 4/29/20. This file is the script for setting up the parameters 
- Plot_jags.R script was added on 4/29/20. This file is the script for plotting outputs. For plotting 2 source isotope plots, such as this project, the user must set up the object jag.1 from the IsotopeR.R script 
- IsotopeR.txt was added on 4/29/20. This file is used when running the IsotopeR.R script  
- IsotopeRgui.R was added 5/1/20. This file is the script for running the Graphical User Interface 
- SampleOutput.Rdata was added on 5/2/20. This file is automatically created after completing a run. It contains the output of this project's data
- FinalFigure.Rmd was added on 5/2/20. This file contains the script to create the final reproduced figure. SampleOutput.Rdata is needed for the script 

## 5/1/20 

After calling the GUI in R, I ran my files through to create a SampleOutput.Rdata file that I could load into my environment. This allowed all the parameters to be set up for this dataset. Looking through the IsotopeRgui.R script I am trying to see if there is a way I can use that to only plot the mixing space and then plot the mixture values over that.

## 5/2/20 

By combining the IsotopeRgui.R and Plot_jags.R scripts I was able to reproduce the figure. I have written the markdown file, FinalFigure.Rmd, that contains the combined scripts and will output the reproduced figure. SampleOutput.Rdata is needed to run the script.  

### Note
It is not necessary for the user to call the IsotopeR GUI as all the model parameters will be set from the SampleOutput.Rdata file  
