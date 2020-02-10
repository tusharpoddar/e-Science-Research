# Research Work
The following research uses the VGGish model definition given by tensorflow in the Audioset models which is an audio classifier model that was trained on the Youtube 8M dataset.  
## Vggish Model - 
#### Things done with the Vggish model on github to see what happens and how does the model work and how does it takes the input and what does it returns. 
1. The vggish_input.py is the file that takes in the wave-file and then returns the 3d shape or in other words it gives out the representation of the data that we feed it. 
2. Vggish_inference_demo.py is the package in the model that uses the definition of the functions in the input file to read a wav file and then process it.  
3. In order to test the model for different models we need to change the global variables defined for the model - vggish_params.AUDIO_EMBEDDING_FEATURE_NAME
4. Mel-features is used to plot the input video to the Convert array into a sequence of successive possibly overlapping frames

Note - The vggish model is written using the older tensor-flow model. As of now we are usng this older version but in the future we plan to update the definition of the model based on newer version of TensorFlow.

## Steps to start different projects in the mac - 
### Set up the conda command on terminal 
- To do this install conda from -  https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html
- After you install Anaconda on the desktop you export the location of your downloaded package in your bash_profile in order for it to load every time you start the terminal. 
- Now you source your bash_profile to load all the changes made in the terminal 
- Now use conda init to start using the environment you create. Download different packages that will be local to that environment. 

### Working with jupyter notebooks using the environment you just created - 
- Jupyter might not be installed in the environment you are working and hence you need to download it using the conda install command. 
- Then you type jupyter notebook - this opens a localhost on you browser and you can run the .ipynb file there. 
- Jupyter is a good way to share code along with the results making it easy for the person viewing it easy. 

## Basic definitions and concepts to be familiar with before going forward with the work - 

1. PCA - 
- The main idea of principal component analysis (PCA) is to reduce the dimensionality of a data set consisting of many variables correlated with each other, either heavily or lightly, while retaining the variation present in the dataset, up to the maximum extent.
- As a layman, it is a method of summarizing data.
- Source- https://www.dezyre.com/data-science-in-python-tutorial/principal-component-analysis-tutorial

## Working with conda
- In order to make the correct environment for the research thing to work install the packages that have been specified in the vggish model information. (For reference of all the packages and their versions are listed in the package-list.txt) OR 
- You can also use the command ```conda create --name <env> --file <package-list.txt>``` to direclty install all of these packages into your environment.
- Once done with that, run the vggish_inference_demo.py first without any changes to run it with the default things. 
- After the things works with the default settings, go on to test your code with the wav file you specify and the file name you want the tf-records to come in. 
- Now we get a tf-record file of the input file and we need to analyse it. This is done on jupyter notebook uploaded in the repository.

