# README Computational Liguistics Final Project (option 2)
OVERVIEW:
For my final project, I chose option 2, making a BERT Question-Answering System. This repo contains the colab where I wrote my code as well as the all_train and all_dev jsons with the data. To run the code, one must first run every cell, and then run the main function. Also, in the load_data function, the file paths currently match where I had the data stored in my google drive in order to be abe to run it locally, so those would have to be changed.

KNOWN BUGS:
I determine a true positive to be a model by checking if a given predicted span matches the actual span, false positives by counting the number of predicted spans that are not in the list of actual spans, and false negatives by counting number all other actual spans that weren't predicted. However, this leads to me getting the exact same values for precision, recall, and F1, which doesn't seem correct. My validation loss after one epoch of training is also higher than that given in the handout, but I had to decrease the batch size to 16 from 64 due to GPU credit issues, which could be a reason behind this.
