Plese get the dataset yourself from https://www.kaggle.com/datasets/kazanova/sentiment140

SET UP AN ENVIRONMENT BEFORE RUNNING THE NOTEBOOK
- install conda 24.5.0 from the shell
- when choosing a kernel in the notebook, set up a new venv with conda 3.11.5 (compatibility issues cos of dropped support in newer versions)

Directory help:
./best_model.h5                                 >>> our best model in hdf5 file
./preoprocessing-and-training.ipynb             >>> preprocessing and training of the best model
./predicting.ipynb                              >>> predicting with our best model
./OLD-preprocessing-training-predicting.ipynb   >>> our old notebook used for training our first model
./OLD_sentiment_analysis_model.h5               >>> our old model
./training.1600000.processed.noemoticon.csv     >>> the original dataset (from kaggle, sentiment140)
./text_save.csv                                 >>> a save of the preprocessed dataset

Compatibility note:
for auto-tuning our hyperparameters, we used the Adam optimiser. For Apple Silicon use keras.optimizers.legacy.Adam, if Intel use keras.optimizers.Adam.
