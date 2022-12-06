# COVID-Detection-with-Ensemble

### Setting environment :

Link to the dataset:
Download the dataset from this link "https://drive.google.com/drive/folders/1j95dLLZadzyQ-MvOHq_W4Qs_9FpXEAE4".
Structure of Dataset:
- Covidx-data
 - test (images for testing)
 - train (images for training)
 - test.txt
 - train.txt 

Clone this repository:
git clone "https://github.com/pearljain7/COVID-Detection-with-Ensemble.git"
Use ``Kaggle`` to run the python notebooks on the given dataset.
On Kaggle:
 - Create a new project.
 - Upload the dataset given.
 - Upload the chosen notebook for either of the five models or the Ensemble model.

## Find best Params using Grid Search:

* Run the chosen model for grid search to gauge the optimal learning rate and Optimiser.
* Analyse the value and find the values for the learning rate (Eg: 0.01) and Optmiser (Eg: SGM).
* Feed this value back into your model to train the model on these values.

## Workflow to train and test the model:
* Train the chosen the chosen model on the given dataset to classify as 'Positive' and 'Negative'. (Note: You need not run grid search again)
* Run the  validation and testing cells and analyse your results.
* Confusion matrix, validation and testing accuracy and loss graphs are plotted for more analysis purpose.

## Testing the model:
* Choose a given image from the dataset and feed into the prediction variable for each model to find the classification of the particular image.
