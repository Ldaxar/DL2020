# Deep Learning assignment
Deep learning assignment using text data.\
Kaggle source: Kaggle source: https://www.kaggle.com/kazanova/sentiment140

## Structure
- data: this folder stores all the external data used by the notebooks
- models: contains the latest versions of our trained neural network models
- NN.ipynb: Contains the code for creating, training and testing Models
- sentiment_analysis.ipynb: 
- SmallModels.ipynb: 
- SVM.ipynb:


## Usage
Before running any of the code, download the data files through the following links

1. [Vectorized tweets](https://drive.google.com/open?id=18smtUq8PjLiiHREXNbdLiA93vc61yTQf)
2. [Processed tweets but not vectorized](https://drive.google.com/open?id=1-3lesjyVd1gGnjJGz_cipqO8CNeiTiPx)
3. [GloVe pre-trained word embeddings](http://nlp.stanford.edu/data/glove.6B.zip)

### BaseModels.ipynb
Before this can be run, "vec.csv" must exist in data folder. "vec.csv" can be downloaded from the link above, or generated from sentiment_analysis.ipynb.
Both Hashed and non-hashed data can be obtained by following the instruction in sentiment_analysis.ipynb. 
Base dataset should also be present in data folder. 
Cells should be run sequentially, and will generate result graphs seen in fig.1 of report. 

### NN.ipynb
Before you can start creating, training or evaluating a model, run the first two cells in the notebook. 
This will run all the import and import the twitter data.

#### Creating and training a model
- Run all function definitions in the data cells under part 1 and 2. (These cells contain function definitions for splitting the data and creating models)
- Choose the dictionary and padding size and run the preprocessing functions. (These cells run the functions for splitting the data, we need the training data and targets)
- Point 4 is divided into four parts that each contain 4 code cells. The four parts correspond to each model and can be run separately.
	1. creating the model
	2. training the model
	3. testing the model accuracy
	4. saving the model in the "models" folder
#### Testing a model
- Run all function definitions in the data cells under part 1 and 2. (These cells contain function definitions for splitting the data and creating models)
- Choose the dictionary and padding size and run the preprocessing functions. (These cells run the functions for splitting the data, we need the test data and targets)
- load the models from the files in the "models" folder
- run the get_report function to get a summary of the accuracy, precision, recall, f1-score and support of the model
