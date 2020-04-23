# IsotopeR outputs

### Note
I only included the IsotopeR estimated values output for Run 3 as that run was the best run. The first 2 runs were very off and the estimated values were not close at all to the paper's. 

## Run 1

The plot of raw values of the consumers(grey) and sources(blue and red). 

![]( https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/observations%202.jpeg)



The plot of the estimated mixing space. This does not look like the orginal Figure 5. The bottom mixing space looks correct but the top mixing space looks too big. I have to revist the data and make sure I have entered the values correct for that source

![](https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/mixing%20space%202.jpeg) 

## Run 2

The plot of the raw values looks different then my first run. I had added a measurment error file to see if that was needed. It added error bars for the consumers(grey). The measurment error is the error associated with mass spectrometry. 
 
![](https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/observations%203.jpeg)

The plot of the estimated mixing space looks worse than my first run. Looking back at the raw data plot I see that the measurment error was applied not only to the consumers but also the sources as they have shifted. 

![](https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/mixing%20space%203.jpeg)

## Run 3

The plot of the raw values looks good! I took out the measurment error file as that was a quick experiment. I reread the paper and IsotopeR is supposed to estimate the measurment error. I also took out the discrimination error file as after contacting the author of the paper he said the discrimination error was already included in the isotopic values.
 
![](https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/observations%204.png)

The plot of the estimated mixing space looks good! I compared the estimated  values of each source that was given in the IsotopeR output to the ones in the paper and they are almost excat! I have a smaller standard deviation (SD) than the paper but I do not know why.
 
![](https://github.com/Intro-Sci-Comp-UIowa/biol-4386-project-cdonne/blob/master/output/Images/mixing%20space%204.png)

This is the output that IsotopeR provided. As stated above, the estimated valuesfrom IsotopeR match the ones in the paper besides a smaller SD
