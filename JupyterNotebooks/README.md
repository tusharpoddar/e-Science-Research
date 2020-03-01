## Steps completed to do the first part of the research - 
- Get the data directly from the VGGish without changing the default parameters. 
- Saw that the numpy array presented did not show the data that was marked and showed some data to be present. 
- Changed the parameters 
	1. SAMPLE_RATE = 250000
	2. MEL_MAX_HZ = 30000 
	
This was done so that we dont lose data when we pass it through the VGGish model. 

- Once we got the numpy array, we plotted the spectrogram using xarray, dynamic map and matplotlib. We then compared it with the results of spectrogram prepared by raven. 

After 
