# intensity-dependent-PLQY
jupyter notebook for intensity-dependent PLQY measurements, taking some code from the PLQY analysis code available on the X Drive.

Outputs a dataframe with the columns: Drive Current, Laser Power / cm2, Photon Flux / cm2,   PLQY, absorptance which you can plot or download as a csv however you wish. There is example code in the notebook to plot this. 

Data should be saved in the form:

A folder containing separate folders with data measured at each drive current. These folders should be labelled 'xxx_currentmA_shorttime_longtime_xxx' with the drive current and short & long integration times. E.G: 'sample1_30mA_short100_long3000_1avg'. The code ignores any text on either side of the integration times & current (sample1_ and _1avg in this example).

Within the folders the data should be saved with these file names: 
'short_in'
'long_in'
'short_out'
'long_out'
'bckg'
'long_bckg'
'empty'
'long_empty'


I plan to update this in the future so that the file names can be more flexible. 


## Updated 20/02/25:
- Now also outpus the spectra files at each intensity in a dataframe.
- Updated plotting section to add multiple samples into one subplot
- Separate section to plot spectras at each intensity with a colormap
