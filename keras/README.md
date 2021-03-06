## Keras

The directory contains code to run the models with a Keras implementation and a Tensorlow backend. Code for both single and multitask models are given. For single tasks, one model for each of the three tasks will be computed by running the python script *main_threeTasks.py*. The multitask learning model can be computed with the script *main_multiTaskLearning.py*.

The data is expected to be in a *dataset* folder, in the main repository directory, with three files inside it: *clean_train.txt* for the training dataset, *clean_test.txt* for the testing dataset, and *clean_valid.txt* for the validation dataset. Inside the dataset folder, a *pretrained_vectors* folder is expected, with two files inside it: *vecs_100.txt* and *vecs_300.txt*.

The results will be stored into the *model_results* folder, with one directory created for each model.

    python main_threeTasks.py
    python main_multiTaskLearning.py

## Contents
* `README.md` this file.
* `code/`
    * [models](code/models.py) code to create, train and validated NN models.
    * [utils](code/utils.py) utility functions to run the models.
* [main_multiTaskLearning](main_multiTaskLearning.py) python script to run the multi-task model.
* [main_threeTasks](main_threeTasks.py) python script to train one NN model for each task.

## Dependencies
* Keras : version 2.1.1
* TensorFlow: 1.4.0
* Numpy: 1.13.3
* [Keras contrib](https://github.com/keras-team/keras-contrib) Keras contrib : 0.0.2
* Sklearn : 0.19.1
* [Sklearn crfsuite](https://sklearn-crfsuite.readthedocs.io/en/latest/index.html) Sklearn crfsuite : 0.3.6
* Python 3.5	
