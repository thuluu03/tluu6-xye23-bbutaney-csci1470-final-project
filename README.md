# tluu6-xye23-bbutaney-csci1470-final-project
CNN model for bone classification on the MURA dataset.

### How to run
This program is meant to run with the MURA dataset already downloaded and 
stored in a google drive account. You can edit the file path names to the 
correct location on your drive. 

Then hit run 'run all' or select the cells you want to run. More specific 
information about the functions is provided in the notebook. 

### Code structure 
The cells at the beginning provide the program access to your google drive and 
rearranges the dataset into an ideal way to be processed. move_data() will alter
the original arrangement of the MURA dataset by pulling all the images out and 
storing them into folders labeled by the bone type. 

The load_data() function requires that the images used are only nested under one 
folder. The name of that folder must be the name of one of the x-ray types which 
will be used to discern the onehot encoding. 

preprocess() must be called seperately on both the training and testing dataset.

The code for the model architecture and hyperparameters are called. Then, the 
training and testing epochs are ran. 

This model saves the whole model after running through all epochs. If you ran 
the model previously, it should be saved to the filepath you indicated at the 
top. You can retrive the model from that location and run the evaluation on it. 
The code is given towards the bottom of the notebook. 
