# COVID-Detection-with-Ensemble

### Setting environment :

Link to the dataset:
Download the dataset from this link "https://drive.google.com/drive/folders/1j95dLLZadzyQ-MvOHq_W4Qs_9FpXEAE4".
Structure of Dataset:
- Covidx-data
 - test (images for testing)
 - train (images for training)
 - test.txt (annotations and labels for the training data)
 - train.txt (annotations and labels for the testing data)


Clone this repository:
git clone "https://github.com/pearljain7/COVID-Detection-with-Ensemble.git"
Use ``Kaggle`` or ``Google Colab`` to run the python notebooks on the given dataset.
On Kaggle/Google Colab:
 - Create a new project.
 - Upload the dataset given.
 - Once the dataset is uploaded, you will see your input files in the following directory: ../input/covidx-cxr2/
 - The directory will contain data in the same format as the drive link.
 - Upload the chosen notebook for either of the five models.
 - For the ensemble models, also upload the given .txt files (which are prediction arrays from models) to the ../predarrays folder:
   resnetarr.txt
   vgg3.txt
   xception-pred.txt
   inceptionarr.txt
   efficientNet-pred.txt
   Run the notebook titled covid-x-ray-ensemble-and-examples.ipynb.

## Find best params using Grid Search:

* Run the chosen model from grid search to gauge the optimal learning rate and Optimiser.
* The grid search runs 10 epochs and iterates over each combination of parameters in the grid. 
* If we test 4 learning rates with 3 optimizers, we end up with a total of 12 combinations. 
* The entire process might run for 2-4 hours depending on the model that is running.
* Check the output from the heatmap. Choose the optimizer and learning rate with the best performance.
* Analyse the value and find the values for the learning rate (Eg: 0.01) and Optimizer (Eg: SGM).
* Feed this value back into your model to train the model on these values.

## Workflow to train and test the model:
* Train the chosen the chosen model on the given dataset to classify as 'Positive' and 'Negative'. (Note: You need not run grid search again)
* Run the  validation and testing cells and analyse your results.
* The validation and training accuracy plot describes how the model performance changes with an increase in epochs.
* The validation and training loss plot describes how the model loss changes with an increase in epochs.
* The confusion matrix and AUC curves help describe the precision and recall on the test dataset.

## Testing the model:
* Choose a given image from the dataset and feed into the input layer of the model to find the classification of the particular image.
