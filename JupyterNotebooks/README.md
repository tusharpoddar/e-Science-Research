# Step One of the research - 
Making sure that I get all the data from the Vggish model and see if the spectrogram produced by the data is similar to the one produced by Raven. 

## Steps completed to do the first part of the research - 
- Get the data directly from the VGGish without changing the default parameters. 
- Saw that the numpy array presented did not show the data that was marked and showed some data to be present. 
- Changed the parameters 
	1. SAMPLE_RATE = 250000
	2. MEL_MAX_HZ = 30000 
	
This was done so that we dont lose data when we pass it through the VGGish model. 

- Once we got the numpy array, we plotted the spectrogram using xarray, dynamic map and matplotlib. We then compared it with the results of spectrogram prepared by raven. 

Another problem that had to be solved in the 

After getting almost the same results from Raven our next step is to plot these differnt spectrograms on a graph and see if the ones that are simililar to to one another are plotted close to each other. For this I had to change the length of the window so that I get the smallest window which shows the labled piece of the spectrogram. This in turn will also help us to cluster the similar spectrograms(representing similar data) together in the final plot. 
